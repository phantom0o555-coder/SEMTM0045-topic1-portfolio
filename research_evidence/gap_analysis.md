# Gap Analysis
## Topic 1: Evaluation under Uncertainty and Limited Data

This document outlines the main research gap identified from the literature reviewed for Theme 2, Topic 1: *Evaluation under Uncertainty and Limited Data*.

---

## 1. What the current literature already does well

The current literature provides strong methodological foundations for understanding model evaluation under constrained data conditions.

First, major methodological papers show that cross-validation is not a single fixed method, but a family of procedures with different bias-variance trade-offs, computational costs, and selection purposes. This means that evaluation design should be matched to the problem rather than chosen by habit.

Second, several studies clearly demonstrate that uncertainty estimation in cross-validation is difficult. In particular, the literature shows that the variance of k-fold cross-validation cannot be estimated in a universally unbiased way, and that naive treatment of fold-wise estimates as independent observations can lead to underestimation of uncertainty.

Third, the literature also shows that evaluation error is not limited to model fitting. Model selection itself can introduce overfitting and selection bias, meaning that optimistic performance estimates may arise before final testing is even performed.

Fourth, more applied studies provide empirical support for these concerns. Real-world examples show that in small-sample settings, single train/test splits may produce unstable results, while repeated cross-validation and bootstrap-based procedures often produce more stable estimates.

Finally, literature on imbalanced classification highlights that metric choice matters. Accuracy and even ROC-based summaries may fail to capture the quality of minority-class prediction, which is especially important in constrained-data scenarios where imbalance is common.

---

## 2. What remains insufficiently addressed

Although the literature recognises that limited data can make model evaluation unstable, several important issues remain insufficiently addressed.

A major limitation is that many studies still focus primarily on average performance estimates rather than on the practical consequences of uncertainty. In many cases, uncertainty is acknowledged but not integrated into the final interpretation of model comparison.

In addition, the joint effect of limited sample size and class imbalance is not always examined in a systematic way. These two constraints often occur together in practice, yet they are frequently discussed in separate methodological conversations.

Another gap is that many studies focus on whether an evaluation method reduces variance, but fewer studies ask whether different validation procedures actually change the reliability of model ranking. In practical machine learning workflows, the question is often not only “how high is the score?” but also “would I select the same model if I used a different validation design?”

There is also a practical gap between theoretical warnings and reporting guidance. The literature explains why evaluation can be misleading, but it provides less consistent guidance on how uncertainty-aware reporting should be structured in small and imbalanced datasets.

Finally, some applied studies address instability in domain-specific settings, but there is still a need for a clearer framework that connects methodological theory, metric choice, resampling strategy, and practical reporting recommendations in one coherent evaluation design.

---

## 3. Why this gap matters

This gap matters because unreliable evaluation can lead to unreliable model selection.

If performance estimates are unstable, overly optimistic, or insufficiently uncertainty-aware, researchers may select models on the basis of noise rather than evidence. This has practical consequences: a model may appear strong during development but fail to generalise under realistic deployment conditions.

The problem becomes more serious in limited-data settings, where each split, fold composition, or class distribution can have a stronger influence on the final estimate. In such situations, reporting only a mean score may create a false sense of confidence.

This issue is not only technical but also methodological and ethical. Poor evaluation design may support claims that are not sufficiently justified, especially in applied domains where model outputs may affect high-stakes decisions.

---

## 4. The research gap identified for this portfolio

Based on the reviewed literature, the main research gap for this portfolio is as follows:

> While prior research has shown that model evaluation becomes unstable under limited-data conditions, there remains insufficient integration of uncertainty-aware reporting, imbalance-sensitive metric selection, and validation-protocol comparison into a single practical evaluation framework for classical machine learning models.

More specifically, the literature does not yet provide a sufficiently clear and practically structured answer to the following question:

> How should classical machine learning models be evaluated in limited and imbalanced data settings so that model comparison is not only more stable, but also more transparent and trustworthy?

---

## 5. Proposed response to the gap

This portfolio responds to the gap by proposing a methodology that compares common evaluation protocols for classical machine learning models under limited and imbalanced data conditions.

Rather than focusing only on predictive performance, the proposed study will examine:
- the stability of performance estimates,
- the effect of class imbalance on metric interpretation,
- the role of uncertainty-aware resampling strategies,
- and the importance of reporting practices that go beyond single average scores.

The goal is not to propose a new predictive algorithm, but to propose a more reliable and transparent evaluation framework for constrained-data settings.

---

## 6. Link to report structure

This gap analysis will directly inform the following sections of the report:
- **Critical Literature Review**
- **Research Gap and Objectives**
- **Proposed Methodology**
- **Practical Considerations and Reporting Implications**
