# Targeted changes

Original cell numbers are one-based. Original source is preserved separately, with outputs and notebook metadata removed.

- Cell 2: `pd.read_csv('D1.csv')` → `pd.read_csv('data/D1.csv').shape`
- Cell 3: `D1 = pd.read_csv('C:\\Users\\HELIOSPHERE\\D1.csv')` → `D1 = pd.read_csv('data/D1.csv')`
- Cell 4: `df = pd.read_csv('D1.csv')` → `df = pd.read_csv('data/D1.csv')`
- Cell 10: `df['insurance'] = df['insurance'].astype(bool)` → `df['insurance'] = df['insurance'].astype('boolean')`
- Cell 20: `df['age_midpoint'] = df['age'].apply(calculate_midpoint)` → `df['age_midpoint'] = df['age'].apply(calculate_midpoint)`
- Cell 44: `reverse_insurance_map = {0: 'no', 1: 'yes'}` → `df['insurance'] = D1['insurance'].copy()`
- Cell 83: `unique_values_count = data['income'].value_counts(dropna=False)` → `unique_values_count = df['income'].value_counts(dropna=False)`
- Cell 84: `data_cleaned = data[data['income'].notna()]  ` → `data_cleaned = df[df['income'].notna()]  `
- Cell 86: `unique_values_count = data['smoking'].value_counts(dropna=False)` → `unique_values_count = df['smoking'].value_counts(dropna=False)`
- Cell 104: `median_contacts = df['worried'].median()` → `median_contacts = df['worried'].median()`
- Cell 111: `df['risk_infection'] = df['risk_infection'].round().astype(int)` → `df['risk_infection_display'] = df['risk_infection'].round().astype('Int64')`
- Cell 112: `df['risk_infection'] = df['risk_infection'].replace(57.999, 58).astype(int)` → `df['risk_infection_display'] = df['risk_infection_display'].replace(57.999, 58)`
- Cell 113: `dg = sns.countplot(data=df, x='risk_infection')` → `dg = sns.countplot(data=df, x='risk_infection_display')`
- Cell 120: `df.to_csv('D1-processed.csv', index=False)` → `df.drop(columns=['risk_infection_display']).to_csv('data/D1-revised.csv', index=False)`
- Cells 65, 95, 114: plotting compatibility, mean syntax, and exclusion of display-only feature.
- Added Markdown, alcohol histogram, skewness table and final categorical/selection audit.
- Count plots: explicit colour for compatibility with installed Seaborn/Matplotlib.
- Original code archive retains all 126 source cells, including the original machine-specific path; it is not intended to run unchanged.
