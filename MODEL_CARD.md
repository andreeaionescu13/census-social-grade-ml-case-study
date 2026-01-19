# Model Card – Census Social Grade Prediction

## Model Overview

This project explores multiple **machine learning models** to analyse and predict
**approximated social grade categories** using census-style socio-economic data.

Rather than focusing on a single final model, the project evaluates **several
learning paradigms** to understand model behaviour, strengths, and limitations
when applied to complex and sensitive socio-economic information.

---

## Models Included

The following model types are explored:

### Supervised Learning – Classification
- Linear and non-linear classifiers for predicting discrete social grade categories
- Evaluation focuses on class-level performance and imbalance sensitivity

### Supervised Learning – Regression
- Regression models for predicting continuous socio-economic indicators
- Used to assess explanatory power and feature relevance

### Unsupervised Learning – Clustering
- Clustering algorithms to identify latent population segments
- Used for exploratory analysis rather than prediction

---

## Intended Use

This project is intended for:
- Educational purposes
- Portfolio demonstration of machine learning workflows
- Analytical exploration of socio-economic data

It is **not intended** for:
- Automated decision-making
- Policy implementation
- Individual-level profiling or classification

---

## Training Data

The models are trained on a **census-style dataset** containing demographic,
household, and lifestyle attributes.

Key characteristics:
- Mixed numerical and categorical features
- Missing values and noisy proxies
- Approximated social grade target variable

The dataset is **not included** in this repository due to redistribution
constraints.

---

## Evaluation Metrics

Model evaluation uses metrics appropriate to each learning paradigm:

### Classification
- Accuracy
- Precision, recall, and F1-score
- Confusion matrix analysis

### Regression
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² score

### Clustering
- Internal validation metrics
- Qualitative interpretation of cluster composition

---

## Performance Summary

Overall model performance highlights several important observations:

- Predictive performance is constrained by class imbalance and proxy variables
- No single model consistently outperforms others across all social grades
- Results emphasise the complexity of modelling socio-economic phenomena

Performance is therefore interpreted qualitatively rather than as a benchmark
for deployment.

---

## Limitations

- Social grade is an approximated construct, not a direct measurement
- Proxy features may encode historical or societal biases
- Class imbalance affects minority group performance
- Encoding strategies may impose unintended ordinal assumptions
- Models are exploratory and not validated for real-world use

---

## Ethical Considerations

Predicting socio-economic status involves inherent ethical risks, including:
- Reinforcement of existing inequalities
- Potential misuse in profiling or exclusion
- Lack of transparency in automated systems

This project explicitly acknowledges these risks and treats model outputs as
**analytical insights**, not actionable decisions.

---

## Caveats and Recommendations

- Results should not be interpreted as objective measures of individual status
- Any real-world application would require extensive fairness, bias, and impact
  assessment
- Explainability techniques are strongly recommended for future extensions

---

## Contact

**Andreea Ionescu**  
AI & Machine Learning Graduate  
Portfolio Project
