# Census Social Grade Prediction – Technical Report

## 1. Problem Overview

Socio-economic classification plays a central role in understanding population
structure, inequality, and access to resources. Social grade indicators are
frequently used in public policy, market research, and social science to analyse
patterns related to income, employment, education, and living conditions.

This project investigates the application of **machine learning techniques**
to predict and analyse **approximated social grade categories** using
demographic and household-level census data. The primary goal is not to optimise
predictive performance, but to **evaluate model behaviour, interpretability,
and limitations** when applied to complex socio-economic data.

---

## 2. Dataset Summary

The dataset consists of census-style observations describing individuals or
households through a combination of numerical and categorical attributes.
These attributes act as proxies for socio-economic status and living standards.

Key dataset characteristics include:
- Mixed data types (numerical and categorical features)
- Presence of missing values
- Potentially correlated socio-economic indicators
- An approximated social grade target variable

Such characteristics reflect real-world census data challenges and motivate
careful preprocessing and model evaluation strategies.

---

## 3. Exploratory Data Analysis

Exploratory analysis was conducted to gain an initial understanding of the data
distribution and feature relationships.

Key observations include:
- Uneven distribution of social grade categories, indicating class imbalance
- Strong variation across demographic and household-related features
- Presence of outliers in several numerical attributes
- Weak linear correlation between individual features and social grade, suggesting
  non-linear relationships

EDA informed both preprocessing decisions and model selection, highlighting the
need for algorithms capable of capturing complex interactions.

---

## 4. Data Preparation and Preprocessing

Data preprocessing was a critical component of this analysis to ensure model
stability and meaningful evaluation.

The following steps were applied:

- **Missing values** were handled using statistical imputation strategies
  appropriate to feature type
- **Categorical variables** were encoded numerically to enable compatibility
  with classical machine learning models
- **Feature scaling** was applied to numerical attributes where required
- **Outliers** were examined and mitigated to reduce distortion in distance-
  based and linear models
- Separate datasets were prepared depending on the learning paradigm
  (classification, regression, clustering)

These preprocessing choices aimed to balance data integrity, interpretability,
and algorithmic requirements.

---

## 5. Modeling Strategy

To provide a comprehensive analysis, the project explores multiple machine
learning paradigms.

### 5.1 Classification

Classification models were trained to predict discrete social grade categories.
Several algorithms were evaluated to compare linear and non-linear decision
boundaries.

Model evaluation focused on:
- Accuracy
- Precision, recall, and F1-score
- Confusion matrix analysis

Special attention was paid to minority classes, as misclassification may
disproportionately affect underrepresented social groups.

---

### 5.2 Regression

Regression models were applied to predict continuous socio-economic indicators
derived from the dataset.

The objective was to assess:
- The extent to which available features explain variance in the target
- The suitability of linear versus non-linear models
- Model sensitivity to noise and feature scaling

Performance was evaluated using standard regression metrics such as MAE, MSE,
and R².

---

### 5.3 Clustering

Unsupervised learning was employed to identify latent population segments based
on socio-economic characteristics.

Clustering analysis included:
- Partition-based clustering methods
- Evaluation using internal validation metrics
- Interpretation of cluster composition and separation

This analysis provided complementary insights beyond supervised prediction,
highlighting structural patterns in the data.

---

## 6. Results and Discussion

Results varied across learning paradigms:

- **Classification models** achieved moderate predictive performance, with
  noticeable sensitivity to class imbalance
- **Regression models** demonstrated limited explanatory power, indicating that
  socio-economic status is influenced by factors not fully captured in the dataset
- **Clustering results** revealed partial grouping structures, though cluster
  separation remained weak

Overall, results emphasise the complexity of modelling socio-economic phenomena
and the limitations of relying solely on proxy variables.

---

## 7. Limitations

Several limitations were identified throughout the analysis:

- Social grade is an approximated construct rather than a direct measurement
- Dataset features act as proxies and may introduce bias
- Class imbalance impacts model sensitivity and fairness
- Encoding choices may impose unintended ordinal relationships
- Models are exploratory and not suitable for real-world decision-making

---

## 8. Ethical Considerations

Predicting socio-economic status raises important ethical concerns, including:
- Risk of reinforcing existing biases
- Potential misuse in profiling or exclusionary practices
- Interpretability and transparency requirements

This project treats social grade prediction strictly as an **analytical and
educational exercise**, not as a deployable system.

---

## 9. Future Work

Potential directions for further development include:
- Incorporation of additional socio-economic indicators
- Use of explainable AI techniques (e.g. SHAP, LIME)
- Fairness-aware and bias-mitigation methods
- Temporal analysis using longitudinal census data

---

## 10. Conclusion

This case study presents an end-to-end exploration of machine learning techniques
applied to census-style socio-economic data. While predictive performance is
constrained by data limitations and proxy variables, the analysis provides
valuable insight into model behaviour, interpretability challenges, and ethical
considerations.

The project highlights the importance of cautious evaluation and contextual
awareness when applying machine learning to socially sensitive domains.
