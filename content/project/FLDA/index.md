---
title: Example Project
summary: An example of using the in-built project page.
tags:
- Deep Learning
date: "2016-04-27T00:00:00Z"

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

Neuroimaging data play an important role to help people understand the brain. Statistical modelsin high dimensional settings have been widely used to deal with imaging modalities as StructuralMagnetic Resonance Imaging (sMRI), functional Magnetic Resonance Imaging (fMRI) and Elec-troencephalography (EEG). One critical question is that how to incorporate complex informationabout brain structure and function into the statistical models.

Considering cerebral cortex is the highly convoluted thin sheet, it can be represented as a 2D surfaceembedded in a 3D space, structured with a 2D geodesic distance. A functional principal componentsanalysis (FPCA) approach over this 2D smooth manifold has been proposed (Lila et al. 2016).Similar strategy for different surfaces could be found in (Ettinger et al. 2016). One advantage of thissurface-constrained technique is avoiding the similarity for functionally different areas caused by3D Euclidean distance because those areas may be close to each other if measured with Euclideandistance. However, current approaches only focus on regression settings, and there are no extensionsto incorporate this novel penalty into the classification approaches.

Linear discriminant analysis (LDA) is an well-known method for classification. Its basic strategyis to find projections such that data can be mapped into the most discriminative low-dimensionalsubspace (Fisher 1936; Hastie et al. 2009).  However, classic LDA tend to fail when the numberof predictorspis large relative to the number of observationsn. In such case, penalized LDA has become increasingly popular. Penalized LDA classifier can be derived from three different framworks,which we shall refer to as the Gaussian model, Fisher’s discriminant problem, and the optimal scoringproblem (Hastie et al. 1994; Hastie et al. 1995).  In terms of functional data, a functional Lineardiscriminant analysis (FLDA) based on Gaussian LDA is proposed (James and Hastie 2001). Also,another reference (Chen and Jiang 2018) generalize Fisher’s LDA to a functional version.

In this project, we generalize the surface-constrained to the classification appraoch FLDA in theoptimal scoring framework. This method is suitable for working with functional data distributed overcurved domains and specifically over two-dimensional smooth Riemannian manifolds
