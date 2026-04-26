# SEMTM0045 Portfolio - Theme 2 Topic 1
## Evaluation under Uncertainty and Limited Data

This repository contains my portfolio work for **SEMTM0045**, under **Theme 2, Topic 1: Evaluation under Uncertainty and Limited Data**.

The project focuses on how model evaluation can become unstable, overly optimistic, or insufficiently transparent when machine learning models are developed under limited and imbalanced data conditions. The portfolio reviews relevant literature, identifies a methodological research gap, and proposes a more uncertainty-aware evaluation framework for classical machine learning models.

---

## Research Question

**How reliable are common evaluation protocols for classical machine learning models under limited and imbalanced data, and can uncertainty-aware resampling strategies provide more trustworthy model assessment?**

---

## Objectives

1. Review how current literature evaluates classical machine learning models in limited-data settings.  
2. Critically compare common evaluation protocols such as hold-out split, stratified k-fold cross-validation, repeated cross-validation, and bootstrap-based estimation.  
3. Assess how small sample size and class imbalance affect the stability and trustworthiness of reported performance metrics.  
4. Propose a more transparent and uncertainty-aware evaluation framework for constrained-data settings.  

---

## Repository Structure

### `planning/`
Contains project planning documents, timeline notes, and viva preparation materials.

### `research_evidence/`
Contains reading notes, key paper summaries, gap analysis, methodology sketches, and the paper matrix used to organise the literature review.

### `latex/`
Contains the LaTeX source files used to draft and structure the portfolio report.

### `final_report/`
Contains the final exported PDF version of the portfolio submission.

### `slides/`
Contains short presentation materials prepared for viva discussion.

---

## Research Focus

The portfolio investigates the methodological problem of evaluating machine learning models when data are limited and class distributions may be imbalanced.

Rather than proposing a new predictive algorithm, the project focuses on the reliability of evaluation itself. In particular, it examines:
- whether common validation protocols provide stable performance estimates,
- how uncertainty should be interpreted and reported,
- how metric choice should reflect class imbalance,
- and how evaluation design affects the trustworthiness of model comparison.

---

## Workflow

The work in this repository has been developed over a two-week period. The workflow includes:

1. topic scoping and confirmation of the research question,  
2. literature search and thematic clustering,  
3. close reading of key methodological papers,  
4. identification of a research gap,  
5. design of a proposed evaluation methodology,  
6. drafting of the report sections,  
7. revision, formatting, and viva preparation.  

Git commits are used to document the development process incrementally.

---

## Core Literature Themes

The literature reviewed in this repository is organised around the following themes:
- cross-validation as an evaluation framework,
- uncertainty and instability in limited-data settings,
- selection bias in performance evaluation,
- metric choice under class imbalance,
- and practical validation design in applied machine learning.

---

## Final Submission

The final portfolio PDF will be stored in:

`final_report/SEMTM0045_Topic1_Portfolio.pdf`

---

## Note on Repository Purpose

This repository is intended to document the development process of the portfolio as well as the final written output. It therefore includes planning materials, working notes, and literature evidence in addition to the final report itself.
