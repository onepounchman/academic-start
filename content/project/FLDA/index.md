---
title: Functional linear discriminant analysis for neuroimaging
summary: Develop a functional data analysis technique to analysis brain data
tags:
- Statistical Learning
- Functional Data Analysis
- Neuroimaging
date: "2020-12-2T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 3D mesh nodes of a half brain
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

Neuroimaging data play an important role to help people understand the brain. Statistical modelsin high dimensional settings have been widely used to deal with imaging modalities as Structural Magnetic Resonance Imaging (sMRI), functional Magnetic Resonance Imaging (fMRI) and Elec-troencephalography (EEG). One critical question is that how to incorporate complex information about brain structure and function into the statistical models.

Considering cerebral cortex is the highly convoluted thin sheet, it can be represented as a 2D surface embedded in a 3D space, structured with a 2D geodesic distance. A functional principal components analysis (FPCA) approach over this 2D smooth manifold has been proposed. One advantage of this surface-constrained technique is avoiding the similarity for functionally different areas caused by 3D Euclidean distance because those areas may be close to each other if measured with Euclidean distance. However, current approaches only focus on regression settings, and there are no extensions to incorporate this novel penalty into the classification approaches.

Linear discriminant analysis (LDA) is an well-known method for classification. Its basic strategyis to find projections such that data can be mapped into the most discriminative low-dimensional subspace. However, classic LDA tend to fail when the numberof predictorspis large relative to the number of observationsn. In such case, penalized LDA has become increasingly popular. Penalized LDA classifier can be derived from three different framworks, which we shall refer to as the Gaussian model, Fisher’s discriminant problem, and the optimal scoringproblem. In terms of functional data, a functional Lineardiscriminant analysis (FLDA) based on Gaussian LDA is proposed. 

In this project, we generalize the surface-constrained to the classification appraoch FLDA in theoptimal scoring framework. This method is suitable for working with functional data distributed overcurved domains and specifically over two-dimensional smooth Riemannian manifolds.
