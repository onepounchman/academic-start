---
title: Finding Atrophy Patterns of Grey Matter through Orthonormal Non-negative Factorization
summary: Utilize matrix factorization and clustering technique to detect the subgroups of disease
tags:
- Matrix Factorization
- Clustering
- Neuroimaging
date: "2020-11-1T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Working pipeline of our fraework
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

Alzheimer’s disease (AD) is characterized by widespread cerebral volume loss (atrophy) at autopsy and structural MRI (sMRI). It is also a devastating neurodegenerative disease, and currently there is no disease-modifying treatment available. It has become increasingly clear that AD is a heterogeneous disease with varying symptoms, cognitive deficits, rates of progression, and anatomic localization within the brain. Some studies have suggested that the spatial distribution of atrophy varies across Alzheimer’s Disease subtypes, and that the gray matter (GM) volume loss patterns may be useful to investigate the heterogeneity in AD. Therefore, the ability to quantify and group the varying patterns of atrophy in AD patients might be helpful to improve our understanding of disease processes.

Recent advances in data-driven methodologies provide automated and interpretable ways to find spatial patterns in the population of subjects. Cortical thickness–based clustering approaches have been investigated with machine learning algorithms to suggest AD subtypes. Previous studies have also used estimates of grey matter from sMRI to identify subtypes. A data-driven Bayesian framework using latent Dirichlet allocation (LDA) was used to estimate latent AD atrophy factors and for each subject and multiple atrophy patterns have been estimated rather than assigning each participant to a single subtype. In other work, a non-linear semi-supervised learning algorithm was used to reveal heterogeneity in AD. These studies often employ clustering methods that only rely on the global similarity of atrophy patterns amongst individuals, which may not be able to identify particular atrophy patterns of a subset of individuals. Non-negative matrix factorization is a matrix factorization approach that a non-negative data matrix is approximately decomposed into the product of two low-rank non-negative matrices. It has been used for dimension reduction but also can be employed in clustering. Therefore, this technique is particularly suitable for atrophy subtype discovery. It was used to identify atrophy subtypes in Alzheimer’s disease dementia, and identified atrophy subtypes were compared based on clinical, biological and cognitive characteristics. One study has used a combination of brain volumes from MRI and neuropsychological assessments in a non-biased fashion and proposes a coupled non-negative matrix factorization (c-NMF) framework to compute phenotyping. Recently, some researchers have developed a modified version of NMF, called orthonormal projective non-negative matrix factorization (OPNMF), and applied it to neuroimaging data. This approach provides components that could be considered as abiologically more meaningful parts-based representation of the disease as compared to more standard approaches. Hence, OPNMF, as a relatively new approach for feature extraction techniques of neuroimaging data, has potential to provide different perspectives for discovering atrophy components.

In this study, we explore the heterogeneity of atrophy patterns in AD using a data-driven framework which yields multiple distinct localized components of gray matter atrophy. We are interested in extracting biologically meaningful components and measuring their association. For this purpose, we quantify subject-level loss coefficients with non-negative least squares and regard them as reflection of how the corresponding components contribute to atrophy loss. We show the ability of those coefficients to distinguish diagnosis groups. Considering the normality assumption may not hold, we assess their correlation of Alzheimer’s disease using Gaussian copula graphical models (GCGMs) rather than ordinary Gaussian graphical models (GGMs). Finally, we use a hierarchical agglomerative cluster analysis to find potential subtypes for each AD subject.
