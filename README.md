# MLvsMELD3

This repository contains code to reproduce the results presented in the paper 

> **Charu V, Liang JW, Mannalithara A, Kwong AJ, and Kim, WR. Human versus artificial intelligence: Head-to-head comparison of predictive performance of MELD 3.0 and machine learning models. 2024.**

## Analyses
- **Analysis 1**: MELD 3.0 variables only
- **Analysis 2**: no variable caps
- **Analysis 3**: no variable caps + additional clinical variables  

## R package dependencies
- Data wrangling and visualization: [`tidyverse`](https://cran.r-project.org/web/packages/tidyverse/index.html), [`compareC`](https://cran.r-project.org/web/packages/compareC/index.html), [`kableExtra`](https://cran.r-project.org/web/packages/kableExtra/index.html), and [`gtsummary`](https://cran.r-project.org/web/packages/gtsummary/index.html)
- Model fitting: [`survival`](https://cran.r-project.org/web/packages/survival/index.html), [`glmnet`](https://cran.r-project.org/web/packages/glmnet/index.html), [`randomForestSRC`](https://cran.r-project.org/web/packages/randomForestSRC/index.html), [`gbm`](https://cran.r-project.org/web/packages/gbm/index.html), [`xgboost`](https://cran.r-project.org/web/packages/xgboost/index.html), [`CoxBoost`](https://cran.r-project.org/web/packages/CoxBoost/index.html), and [`survivalmodels`](https://cran.r-project.org/web/packages/survivalmodels/index.html)
- Modeling tuning: [`glmnetUtils`](https://cran.r-project.org/web/packages/glmnetUtils/index.html), [`mlr3`](https://cran.r-project.org/web/packages/mlr3/index.html), [`mlr3proba`](https://cran.r-project.org/web/packages/mlr3proba/index.html), [`paradox`](https://cran.r-project.org/web/packages/paradox/index.html), [`mlr3tuning`](https://cran.r-project.org/web/packages/mlr3tuning/index.html), [`mlr3extralearners`](https://github.com/mlr-org/mlr3extralearners), and [`mlr3pipelines`](https://cran.r-project.org/web/packages/mlr3pipelines/index.html)

## Data

US waitlist registry data from the OPTN: 

- Training set (n=20587): data used to develop MELD3.0<sup>[1](#myfootnote1)</sup>, consisting of a 70% random sample of liver transplant candidates newly waitlisted between 1/15/2016 and 12/31/2018
- Test set (n=33443): new registrants between 1/1/2021 and 12/31/2023

---

<a name="myfootnote1">1</a>. Kim WR, Mannalithara A, Heimbach JK, Kamath PS, Asrani SK, Biggins SW, Wood NL, Gentry SE, Kwong AJ. MELD 3.0: the model for end-stage liver disease updated for the modern era. Gastroenterology. 2021 Dec 1;161(6):1887-95. doi.org/10.1053/j.gastro.2021.08.050 
