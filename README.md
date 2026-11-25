# COVID-19 Survey Data Exploration and Mining
QUT IFN509 | Postgraduate group assessment | Team leader | 18.75/20 (93.75%)

## Individual contribution
Proposed task allocation for a three-member team, monitored progress and timelines, supplemented missing analytical work and coordinated meetings.

## Repository guide
- `original_source.ipynb`: all original source cells, unchanged; saved outputs and notebook metadata removed for privacy. Historical reference, not runnable as-is.
- `academic_analysis.ipynb`: original workflow with targeted corrections and English explanations; 106 of 126 original cells retained verbatim (including empty cells).
- `CHANGELOG.md`: correction log.

## Findings
The original dataset contains 5,789 records and 36 variables. The submitted processed dataset contains 4,166 records (24.00% positive), compared with 40.34% in the original. Applying the corrected sequential filters produces 4,100 records (24.07% positive). The difference warrants investigation. The added categorical smoking analysis on the original dataset gives Cramer's V = 0.101 (weak association); this is not causal evidence.

The original assessment proposed classification and derived risk indices; it did not train a predictive model. The later validation section is separate from the graded work.

## Run locally
Install `pip install -r requirements.txt`, place authorised copies of D1.csv and D1-processed.csv in data/, then run `jupyter lab` from this directory and open academic_analysis.ipynb. Run all cells. The revised notebook was executed successfully; saved outputs are intentionally excluded from public files. Do not publish the CSVs, raw outputs or team materials without permission.

## Portfolio report
See `Portfolio.pdf` for the English academic case study. `figures/` contains aggregate charts recalculated from the supplied CSVs. No machine learning or dashboard is included in this academic-only release.
