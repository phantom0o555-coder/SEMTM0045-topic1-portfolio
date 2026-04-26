# Literature Notes
## Topic 1: Evaluation under Uncertainty and Limited Data

This document contains working notes from the literature review process. The purpose is to organise the main ideas, recurring themes, and emerging patterns across the papers selected for the portfolio.

---

## 1. Main literature clusters

After reviewing the selected papers, the literature can be grouped into four main clusters.

### Cluster A: Cross-validation as an evaluation framework
These papers explain the role of cross-validation and how different procedures serve different purposes.

**Relevant papers**
- Arlot & Celisse (2010)
- Yates et al. (2022/2023)

**Main idea**
Cross-validation should not be treated as a single standard method. Different protocols involve different trade-offs and should be chosen according to the evaluation objective.

---

### Cluster B: Uncertainty, variance, and instability in limited-data evaluation
These papers focus on the fact that evaluation results can become unstable when data are limited.

**Relevant papers**
- Grandvalet & Bengio (2004)
- Nadeau & Bengio (2003)
- Varoquaux (2018)
- Zantvoort et al. (2024)

**Main idea**
Performance estimates in small datasets are often much less stable than they appear. Variance can be difficult to estimate correctly, and uncertainty may be underestimated in common reporting practice.

---

### Cluster C: Selection bias and over-optimistic evaluation
These papers show that bias can enter not only through data splitting, but also through the model selection process itself.

**Relevant papers**
- Cawley & Talbot (2010)

**Main idea**
Evaluation problems are not restricted to the final testing stage. Selection procedures can overfit noisy validation estimates and produce inflated performance claims.

---

### Cluster D: Imbalanced data and metric choice
These papers highlight the importance of choosing metrics that reflect the actual prediction goal when data are imbalanced.

**Relevant papers**
- Saito & Rehmsmeier (2015)
- Zhao et al. (2025)

**Main idea**
Evaluation reliability depends not only on resampling protocol, but also on whether the chosen metrics capture the problem appropriately. In imbalanced settings, some commonly used metrics may be insufficient or misleading.

---

### Cluster E: Applied and practical validation design
These papers connect theoretical concerns to practical real-world evaluation design.

**Relevant papers**
- Singh et al. (2021)
- Allgaier & Pryss (2024)

**Main idea**
Real applications show that evaluation design has substantial effects on performance stability and external validity. Validation procedures should reflect real data structure rather than convenience alone.

---

## 2. Main recurring themes across the literature

### Theme 1: Average performance is not enough
A repeated theme in the literature is that reporting only an average score can conceal important instability. The reliability of the estimate matters as much as the value of the estimate itself.

### Theme 2: Limited data amplifies methodological weaknesses
When sample size is small, each split, fold, or class composition matters more. Small data magnifies the consequences of poor evaluation design.

### Theme 3: Validation design affects interpretation
Different protocols can lead not only to different levels of variance, but also to different practical conclusions about model quality.

### Theme 4: Metric choice is part of evaluation design
Evaluation is not only about how to split data but also about what performance indicator is reported. This is especially important when datasets are imbalanced.

### Theme 5: Practical reporting guidance is still underdeveloped
The literature identifies many methodological dangers, but more explicit guidance is still needed on how to report model performance transparently under constrained-data conditions.

---

## 3. Important observations for my report

### Observation 1
The literature strongly supports the idea that limited-data model evaluation is inherently uncertain rather than simply noisy.

### Observation 2
There is a difference between reducing variance and improving trustworthiness. A procedure may appear more stable while still failing to support transparent interpretation.

### Observation 3
The interaction between limited sample size and class imbalance is highly relevant but not always treated in a fully integrated way.

### Observation 4
The most useful contribution for my report is not to propose a new algorithm, but to propose a better framework for evaluation and reporting.

---

## 4. Preliminary synthesis

The literature suggests that the central challenge is not simply to identify the “best” validation method, but to design a more trustworthy evaluation process.

This includes:
- choosing a validation protocol appropriate to the data setting,
- choosing metrics appropriate to the class structure,
- acknowledging uncertainty rather than hiding it,
- and avoiding overconfident performance claims based on unstable evidence.

This synthesis directly motivates the research gap and the proposed methodology for the portfolio.

---

## 5. Questions guiding further reading

The following questions will guide my continued reading and note-taking:

1. Which evaluation protocols are most defensible under limited-data conditions?
2. How should uncertainty be reported when variance estimates are themselves imperfect?
3. How can class imbalance be incorporated into the evaluation framework rather than treated as a separate issue?
4. How should model comparison be interpreted when different protocols produce different rankings?
5. What reporting framework would make evaluation more transparent and trustworthy?

---

## 6. Working conclusion

The literature reviewed so far supports a clear direction for the portfolio:

The problem is not only that limited data produces unstable estimates. The deeper issue is that standard evaluation practice often fails to communicate uncertainty, sensitivity, and methodological limits clearly enough. Therefore, the portfolio should aim to propose an evaluation framework that is not only more stable, but also more transparent and more appropriate for limited and imbalanced data settings.
