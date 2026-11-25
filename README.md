# COVID-19 Survey Data Analysis & Machine Learning

A postgraduate data science portfolio exploring COVID-19 survey data through exploratory data analysis, statistical validation, unsupervised learning and supervised classification.

## Project Overview

Developed as part of postgraduate coursework at Queensland University of Technology (QUT). The repository contains two complementary analyses of COVID-19 survey data, with English and Japanese portfolio reports.

## Technical Skills

Python · Pandas · NumPy · Matplotlib · Seaborn · SciPy · Scikit-learn · K-modes (K-prototypes) · Jupyter Notebook

## Projects

| Project | Methods | Assessment grade |
| --- | --- | --- |
| [01 — Data Exploration](01-data-exploration/) | Data cleaning, imputation, outlier investigation, correlation analysis, chi-square testing | 93.75% (18.75/20) |
| [02 — Machine Learning](02-machine-learning/) | K-prototypes clustering, logistic regression, cross-validation, GridSearchCV, RFECV, ROC-AUC | 89.5% |

## Key Findings

- The original exploration dataset contains 5,789 records and 36 variables.
- Preprocessing substantially changes the observed proportion of positive cases, highlighting potential selection effects.
- K-prototypes clustering explores patterns across mixed numerical and categorical variables.
- Baseline logistic regression achieved approximately 67.6% test accuracy in the saved notebook results.
- Findings are exploratory and do not establish causation or clinical predictive validity.

## Individual Contribution

For the data exploration group assessment, I served as team leader, proposed task allocation for three members, monitored progress and timelines, supplemented analytical work and coordinated meetings. Subsequent corrections and statistical validation are distinguished from the original graded work in the notebook.

## Portfolio Reports

| Project | English | Japanese |
| --- | --- | --- |
| Data Exploration | [PDF](01-data-exploration/reports/COVID19_Exploration_EN.pdf) | [PDF](01-data-exploration/reports/COVID19_Exploration_JP.pdf) |
| Machine Learning | [PDF](02-machine-learning/reports/COVID19_Analytics_EN.pdf) | [PDF](02-machine-learning/reports/COVID19_Analytics_JP.pdf) |

## Running Locally

See the README in each project directory for setup instructions. Original survey CSV files are excluded; authorised copies are required to reproduce the analyses.

## Limitations and Data Privacy

This repository is an academic portfolio, not a clinical decision-making tool. Survey limitations, missing values, preprocessing choices and model performance constrain interpretation. Original data and third-party academic materials should not be redistributed without permission.
