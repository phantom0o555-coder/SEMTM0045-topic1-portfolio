# Methodology Sketch
## Proposed Study Design for Topic 1: Evaluation under Uncertainty and Limited Data

This document outlines the proposed methodology for the portfolio project. The aim is not to develop a new predictive model, but to design a more reliable and transparent evaluation framework for classical machine learning under limited and imbalanced data conditions.

---

## 1. Study aim

The proposed study aims to investigate how common evaluation protocols behave when applied to classical machine learning models under constrained-data settings.

The central purpose is to examine whether model assessment can be made more trustworthy by combining:
- more careful validation protocol selection,
- uncertainty-aware resampling strategies,
- and metrics that are appropriate for imbalanced data.

---

## 2. Research question

**How reliable are common evaluation protocols for classical machine learning models under limited and imbalanced data, and can uncertainty-aware resampling strategies provide more trustworthy model assessment?**

---

## 3. Proposed objectives

1. To compare common evaluation protocols used for classical machine learning under limited-data conditions.  
2. To examine how small sample size affects the stability of performance estimates.  
3. To assess how class imbalance influences metric interpretation and model comparison.  
4. To propose a more transparent evaluation framework that integrates uncertainty-aware reporting.

---

## 4. Proposed data strategy

The study will use small or down-sampled classification datasets that reflect realistic constrained-data conditions.

### Proposed data characteristics
- supervised classification tasks,
- relatively small sample size,
- potential class imbalance,
- suitability for repeated resampling and comparison across protocols.

### Rationale
The purpose is not to maximise predictive performance on a large benchmark, but to create a setting where the effects of validation design and uncertainty can be observed clearly.

If appropriate, a combination of:
- one or two publicly available real datasets,
- and controlled down-sampled versions of larger datasets

may be used to examine how performance stability changes as sample size decreases.

---

## 5. Proposed models

The proposed study will focus on a small set of classical machine learning models, such as:
- Logistic Regression
- Random Forest
- Support Vector Machine or XGBoost

### Rationale
These models are widely used, interpretable at a methodological level, and sufficient for comparing evaluation procedures without shifting the focus toward architecture engineering.

The goal is to compare evaluation design rather than to optimise a specific algorithm.

---

## 6. Proposed evaluation protocols

The study will compare several common validation approaches:

1. **Single hold-out split**  
2. **Stratified k-fold cross-validation**  
3. **Repeated stratified k-fold cross-validation**  
4. **Bootstrap-based performance estimation**

### Rationale
These protocols represent a range of common approaches from simple but unstable methods to more resampling-intensive procedures.

Comparing them allows the study to assess:
- estimate stability,
- sensitivity to sample composition,
- and practical differences in model comparison.

---

## 7. Proposed metrics

The study will report metrics appropriate for limited and imbalanced classification settings, potentially including:

- F1 score  
- Balanced Accuracy  
- AUROC  
- AUPRC  
- Mean performance across resamples  
- Standard deviation or confidence interval estimates  
- Model ranking consistency across protocols

### Rationale
The inclusion of both central performance measures and uncertainty-related summaries is necessary to reflect not only how well a model performs, but also how trustworthy the estimate is.

Metrics such as AUPRC are especially relevant when class imbalance is present.

---

## 8. Analysis focus

The proposed analysis will focus on the following questions:

### 8.1 Estimate stability
How much do reported performance values vary across different evaluation protocols?

### 8.2 Sensitivity to limited data
Does performance become more unstable as sample size decreases?

### 8.3 Metric interpretation under imbalance
Do different metrics lead to different conclusions when class imbalance is present?

### 8.4 Model ranking consistency
Do different validation procedures produce different conclusions about which model performs best?

### 8.5 Reporting transparency
Would uncertainty-aware summaries provide a more cautious and reliable basis for model comparison than single point estimates?

---

## 9. Expected contribution

The expected contribution of the proposed study is methodological rather than algorithmic.

The project aims to contribute:
- a critical comparison of common evaluation protocols,
- a clearer account of uncertainty in constrained-data settings,
- and a practical framework for more transparent model performance reporting.

The intended outcome is a recommendation-oriented evaluation design rather than a new predictive modelling technique.

---

## 10. Practical considerations

Several practical issues will need to be considered:

- ensuring datasets are suitable for repeated resampling,
- avoiding over-interpretation of unstable estimates,
- selecting metrics appropriate to the data distribution,
- and clearly stating the limits of generalisability.

The final report will also discuss the ethical and methodological risks of overconfident evaluation in small or imbalanced datasets.

---

## 11. Link to report sections

This methodology sketch will support the following sections of the final report:
- **Research Gap and Objectives**
- **Proposed Methodology**
- **Data, Ethics, and Practical Considerations**
- **Non-Technical Summary**
