---
title: Assessment of Antibody Marker Correlates of Risk and Protection 
summary: A clinical trials about Vaccine Efficacy 
tags:
- Clinical Trials
- Machine Learning
- Causal Inference
date: "2020-12-1T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Conditional Risk Curve for Vaccine and Placebo Group Combined based on EIA and PCA markers: Endpoint 1
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
This project focuses on the assessment of anti-F IgG ELISA, Palivizumab-competitive antibody (PCA), and Microneutralization (MN) 50% antibody titers to RSV/A and RSV/B, measured in mothers and their infants, as correlates of risk and as correlates of protection against RSV disease endpoints in infants in RSV-M-301. The correlates analyses are conducted for the South Africa study sites and follow-up period of infants through to 90 days of age. To build ‘estimated optimal surrogates’ based on different specified antibody variable sets, i.e., models that best predict the RSV disease endpoint, we implementation of Superlearner Regression, an ensemble model, to conduct this.

In clinical trials, one is often interested in identifying a biomarker that is predictive of a clinical outcome of interest. In particular, in vaccine efficacy trials, one aims to find so called correlates of protection, such as neutralizing antibody titer, that are indicative of the risk of disease and vaccine efficacy. Such correlates allow one to predict the efficacy of new vaccines by only analyzing immunological measures, as opposed to observing the clinical endpoints. Such analysis generally requires only hundreds, rather than thousands, of participants in the vaccine study, and allows for vaccine efficacy to be assessed efficiently in terms of both economic resources and time. For such purposes, a prominent correlate is the so-called threshold of protection, generally defined as a threshold value of an immune- response biomarker that predicts a low risk of disease, combined with other evidence for a valid surrogate endpoint.We also develop a nonparametric CoR threshold estimation method, using the version accounting for right-censoring of some follow-up times. We develop a nonparametric CoR threshold estimation method which allows adjustment of arbitrary baseline covariates based on TMLE.

