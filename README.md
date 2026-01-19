# Census Social Grade Prediction – Machine Learning Case Study

## Overview

This project presents an **end-to-end machine learning case study** focused on
**predicting and analysing socio-economic (social grade) categories** using
demographic and household-level census data.

The analysis integrates **exploratory data analysis, supervised learning
(classification & regression), and unsupervised learning (clustering)** to
investigate patterns in socio-economic status and evaluate the behaviour of
different machine learning models under realistic data constraints.

The project was originally developed as an **academic coursework assignment**
and later adapted for **professional portfolio presentation**, preserving the
original analytical logic while improving structure, clarity, and
reproducibility.

---

## Objectives

- Explore demographic and household characteristics influencing social grade
- Apply multiple machine learning paradigms to the same real-world dataset
- Compare model behaviour across classification, regression, and clustering tasks
- Highlight limitations, biases, and practical considerations of census-based ML

---

## Dataset

This project uses a **census-style socio-economic dataset** containing
demographic, household, and lifestyle attributes.

The dataset includes:
- Numerical features (e.g. age-related indicators, household metrics)
- Categorical features (e.g. employment, housing, education proxies)
- A target variable representing **approximated social grade**

⚠️ **Important:**  
The dataset is **not included** in this repository due to redistribution and
licensing constraints.

### How to obtain the dataset

1. Obtain the dataset from the original academic source or an equivalent public
   census dataset
2. Place the CSV file locally in:
   ```text
   data/raw/Census.csv
   ```

 
## Methodology

The project follows a structured machine learning workflow:

Exploratory Data Analysis
Distribution analysis of numerical and categorical variables
Identification of missing values and outliers
Initial feature relevance inspection

### Data Preprocessing
Handling missing values using statistical imputation
Encoding categorical variables
Feature scaling and normalization
Preparation of data for different model families

### Supervised Learning
Classification models to predict social grade categories
Regression models to predict continuous socio-economic indicators
Evaluation using appropriate metrics for each task

### Unsupervised Learning
Clustering techniques to identify latent population groups
Cluster validation using internal metrics and visual inspection
Detailed technical steps, figures, and results are provided in report.md.

 ```text
census-social-grade-ml-case-study/
├── README.md
├── report.md
├── MODEL_CARD.md
├── requirements.txt
├── notebooks/
│   └── census_social_grade.ipynb
└── data/
    ├── README.md
    └── raw/
        └── .gitkeep
```

## Reproducibility
To reproduce the analysis locally:
1. Place the dataset in:
```text
data/raw/Census.csv
```
2. Install dependencies:
```text
pip install -r requirements.txt
```
3. Run the notebook:
```text
notebooks/census_social_grade.ipynb
```

## Limitations
Census data contains proxy variables that may not fully capture socio-economic
complexity
Class imbalance affects predictive performance for minority social grades
Encoding choices may introduce implicit assumptions
Models are exploratory and not intended for policy or decision-making use

## Disclaimer
This project is for educational and portfolio purposes only.
It does not constitute social, economic, or policy advice.

## Author
Andreea Ionescu
AI & Machine Learning Graduate
Portfolio Project
