# Key Papers Summary
## Core Literature for Topic 1: Evaluation under Uncertainty and Limited Data

This document summarises the most important papers selected as the core literature foundation for the portfolio. These papers were chosen because they provide the strongest support for the theoretical, methodological, and practical aspects of the report.

---

## 1) Arlot, S. & Celisse, A. (2010)
**Title:** *A Survey of Cross-Validation Procedures for Model Selection*

### Why this paper is important
This paper provides the broad methodological foundation for understanding cross-validation as a family of procedures rather than a single standard method. It is especially useful for structuring the literature review and framing the evaluation landscape.

### Core contribution
The paper explains that different cross-validation procedures involve different trade-offs in bias, variance, and computational cost. It therefore supports the argument that validation design should be chosen according to purpose and data context.

### Relevance to my topic
This paper is central because Topic 1 is fundamentally about evaluation design under uncertainty. It helps define the methodological background before moving into more critical discussion of instability and bias.

### How I will use it
I will use this paper in the **literature review** to introduce the main evaluation protocols and to justify why evaluation design cannot be treated as a routine technical choice.

---

## 2) Grandvalet, Y. & Bengio, Y. (2004)
**Title:** *No Unbiased Estimator of the Variance of K-Fold Cross-Validation*

### Why this paper is important
This is one of the most important theoretical papers for my topic because it addresses uncertainty estimation directly.

### Core contribution
The paper proves that there is no universally unbiased estimator of the variance of k-fold cross-validation. This is highly relevant because it shows that uncertainty in evaluation is not just a matter of reporting more numbers; it is a structural methodological difficulty.

### Relevance to my topic
The portfolio focuses on evaluation under uncertainty, so this paper provides strong support for the argument that performance estimation in limited-data settings is inherently fragile.

### How I will use it
I will use this paper in the **critical literature review** and in the **justification for uncertainty-aware reporting**.

---

## 3) Cawley, G.C. & Talbot, N.L.C. (2010)
**Title:** *On Over-fitting in Model Selection and Subsequent Selection Bias in Performance Evaluation*

### Why this paper is important
This paper expands the discussion beyond train/test splitting by showing that model selection itself can overfit.

### Core contribution
It argues that performance inflation may arise from the model selection process, and that the resulting bias can be large enough to distort conclusions about which algorithm is actually better.

### Relevance to my topic
This paper is essential because it shows that unreliable evaluation is not only a small-data issue but also a process-design issue. This strengthens the case for more rigorous validation strategies.

### How I will use it
I will use this paper in the **literature review** and the **research gap section** to show that evaluation problems arise both before and after final performance reporting.

---

## 4) Varoquaux, G. (2018)
**Title:** *Cross-validation failure: Small sample sizes lead to large error bars*

### Why this paper is important
This is one of the most directly relevant papers to Topic 1 because it focuses explicitly on small sample sizes and unstable evaluation.

### Core contribution
The paper shows that cross-validation error bars can become very large when sample sizes are small, which means that apparently strong model results may be much less reliable than they seem.

### Relevance to my topic
The portfolio centres on uncertainty under limited data, so this paper gives direct support to the argument that small-sample evaluation can easily produce misleading confidence.

### How I will use it
I will use this paper in the **introduction** and **critical literature review** as one of the main sources supporting the project motivation.

---

## 5) Saito, T. & Rehmsmeier, M. (2015)
**Title:** *The Precision-Recall Plot Is More Informative than the ROC Plot When Evaluating Binary Classifiers on Imbalanced Datasets*

### Why this paper is important
This paper is important because it introduces the metric-selection side of the problem. Evaluation reliability is not only about resampling design but also about what is measured.

### Core contribution
The paper argues that PR-based evaluation is often more informative than ROC-based evaluation when class imbalance is strong.

### Relevance to my topic
Limited-data settings frequently include imbalance, so this paper supports the idea that metric choice must be aligned with the data structure and modelling goal.

### How I will use it
I will use this paper in the **methodology section**, especially in the justification of metrics such as precision-recall based evaluation and imbalance-aware reporting.

---

## 6) Singh, V. et al. (2021)
**Title:** *Impact of train/test sample regimen on performance estimate stability of machine learning in cardiovascular imaging*

### Why this paper is important
This paper gives practical empirical evidence that validation design changes the stability of model performance estimates in real small-data contexts.

### Core contribution
It compares multiple validation regimens and shows that single split-sample validation is considerably less stable than repeated cross-validation or bootstrap-based approaches.

### Relevance to my topic
This paper connects theory to practice. It helps show that the concerns raised in methodological papers are not purely abstract.

### How I will use it
I will use this paper in the **literature review** as applied evidence and in the **methodology section** to justify comparing multiple resampling-based evaluation strategies.

---

## Overall role of these key papers

Together, these key papers support the report in the following way:

- **Arlot & Celisse (2010)**: evaluation protocol foundation  
- **Grandvalet & Bengio (2004)**: uncertainty estimation difficulty  
- **Cawley & Talbot (2010)**: selection bias and evaluation distortion  
- **Varoquaux (2018)**: small-sample instability  
- **Saito & Rehmsmeier (2015)**: imbalance-aware metric choice  
- **Singh et al. (2021)**: practical evidence from real data

These six papers form the core intellectual structure of the portfolio and will be prioritised during close reading.
