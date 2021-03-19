---
title: A Multivariate Longitudinal Model Using Multi-task Gaussian Process Regression
summary: Develop a novel a Gaussian process framework for analyzing longitudinaldata with multiple outcomes. 
tags:
- Additive Gaussian Process Regression
- Multi-task Learning
- Longitudinal
date: "2020-12-4T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Sample true and predicted trajectories for a random sample of five people in simulation study
  focal_point: Smart

#links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---

Many modern biomedical research problems are both multivariate and longitudinal. For example, multiple biomarkers or phenotypes are often measured at multiple times during the course of a genetic study. Modeling multivariate outcomes jointly often improves prediction by leveraging the correlations between them, and biomedical outcomes are often correlated.

Previous work has developed a variety of multivariate models for biomedical applications. Such models include a kernel machine-based multivariate regression to facilitate the joint evaluation of multi-biomarker effects on multiple phenotypes; a multivariate microbiome regression-based kernel test for association between multiple continuous outcomes and overall microbiome composition; and a scaled marginal model for genome-wide association analysis of multiple continuous secondary phenotypes in case-control studies. However, these methods do not account for within-subject correlations over repeated measurements in the case of longitudinal data.

On the other hand, a variety of flexible modeling approaches exist for analyzing longitudinal data, but to our knowledge these have been primarily limited to univariate outcomes. The mixed model and the method of generalized estimating equations (GEE) are widely used to address correlation in longitudinal data. Additionally, one extension of linear mixed effects model, called LonGP, is a flexible and interpretable non-parametric modeling framework. In that framework, a GP model can be made additive by defining the kernel function to be a sum of individual and product (interaction) kernels, similar to standard linear models. Multi-task learning is a branch of machine learning for jointly modeling related tasks or outcomes, allowing the tasks to share information and thereby improving predictions in many scenarios. Multi-task Gaussian processes (GPs) are a class of multi-tasking learning methods building upon the standard GP model to learn inter-task dependencies based on the task identities and the observed data for each task. The learned inter-task dependencies are represented by a positive semi-definite task-similarity matrix which can be used in conjunction with a covariance function over the input features. Nonparameteric methods such as GPs make fewer assumptions about the underlying data generating mechanisms.

Therefore, this work proposes a general framework for analyzing longitudinal data with multiple outcomes. We combine an additive GP framework with multi-task learning to handle multivariate longitudinal data.
