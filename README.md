# LASSO and Ridge Regression — A Comparative Study

<!-- badges: start -->
![Python](https://img.shields.io/badge/Python-3.11+-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)
[![Medium](https://img.shields.io/badge/Medium-@vadimtyuryaev-green?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@vadimtyuryaev)
<!-- badges: end -->

This repository provides a **fully executed Jupyter notebook** (`src/notebooks/L1_L2_Regression.ipynb`) illustrating the **mathematical derivation, geometric interpretation, and computational implementation** of two cornerstone regularization techniques in statistical learning:
* **LASSO (L1)** regression.  
* **Ridge (L2)** regression.  

The notebook bridges theoretical foundations with empirical experimentation, serving as both an instructional and exploratory resource for **data scientists, statisticians, and students of machine learning** interested in understanding the role of regularization in high-dimensional modeling.

---

## Core Concepts Covered

| # | Topic | Summary |
|---|--------|----------|
| 1 | **The Big Data Challenge** | Motivates the need for regularization under multicollinearity and high-dimensionality, with motivating examples. |
| 2 | **Variable Selection Methods** | Reviews classical subset-selection techniques (best subset, forward, backward) and their computational limitations. |
| 3 | **Ordinary Least Squares (OLS)** | Derives the OLS estimator and introduces the need for penalized estimation. |
| 4 | **LASSO Regression (L1 Regularization)** | Presents the derivation of the soft-thresholding operator, explores sparsity induction, and visualizes the diamond-shaped constraint geometry. |
| 5 | **Ridge Regression (L2 Regularization)** | Derives the analytical closed-form solution, interprets shrinkage effects, and contrasts it with LASSO’s sparsity behavior. |
| 6 | **Elastic Net** | Demonstrates a convex combination of L1 and L2 penalties |
| 7 | **Confidence Intervals** | Discusses the breakdown of classical inference under penalization and emerging approaches for post-selection inference. |
| 8 | **Lambda (λ) Selection** | Implements automated hyperparameter tuning via **Bayesian Optimization**, balancing bias–variance trade-offs. |

---

## Learning Objectives

- Understand the statistical motivation for regularization in linear models.  
- Visualize the effect of L1 penalty on coefficient shrinkage.  
- Explore the **geometry of constraint regions** in two-dimensional parameter space.
- Derive and analyze the OLS, LASSO, and Ridge estimators from **first principles**.
- Learn why standard hypothesis testing **assumptions break down** in the context of LASSO regularization and model selection.
- Learn how modern optimization and **Bayesian** search methods automate regularized model selection . 

---

## View Online

The rendered notebook is publicly available at:

👉 [**vadimtyuryaev.github.io/LASSO**](https://vadimtyuryaev.github.io/LASSO/)

---

## Suggested R Software Packages

| Package | Description |
|----------|--------------|
| [**selectiveInference**](https://cran.r-project.org/web/packages/selectiveInference/index.html) | Performs **post-selection inference** for models such as the LASSO, leveraging the *polyhedral lemma* framework. Enables valid hypothesis testing and confidence interval estimation after variable selection. |
| [**RegrCoeffsExplorer**](https://cran.r-project.org/web/packages/RegrCoeffsExplorer/index.html) | Provides **interactive visualization of regression coefficients and confidence intervals**, allowing intuitive exploration of model stability and the effects of regularization. |

---

## Suggested References

- Hastie, T., Tibshirani, R., & Friedman, J. (2009). *The Elements of Statistical Learning.* Springer. 
- Hoerl, A. E., & Kennard, R. W. (1970). *Ridge Regression: Biased Estimation for Nonorthogonal Problems.* *Technometrics*, **12(1)**, 55–67.   
- Lee, J. D., Sun, D. L., Sun, Y., & Taylor, J. E. (2016). Exact Post-Selection Inference, with Application to the LASSO. Annals of Statistics, 44(3), 907–927.
- Tibshirani, R. (1996). *Regression Shrinkage and Selection via the Lasso.* *Journal of the Royal Statistical Society: Series B*, **58(1)**, 267–288.  
- Taylor, J., & Tibshirani, R. J. (2018). Post-Selection Inference for ℓ₁-Penalized Likelihood Models. Canadian Journal of Statistics, 46(1), 41–61.
