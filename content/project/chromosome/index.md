---
title: Chromosome Classification with Convolutional Neural Network 
summary: Develop a deep learning based model to classify chromosome images
tags:
- Deep Learning
- Computer Vision

#date: "2020-12-1T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: CNN architecture used for chromosome classification
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
The human cell normally contains 23 pairs of chromo- somes, including 22 pairs of autosomes (the ones exist in both males and females) as well as sex chromosomes X and Y. Females have double X chromosomes as one pair of sex chromosomes, while males have both X and Y. Chromosome abnormality, namely aneuploidy (having abnormal number of chromosomes in a cell) and structural abnormalities (including deletions, duplication, translocation, inversion, insertions rings, and isochromosome) may cause genetic disorder such as Down’s syndrome. It is important to inspect the cells of a patient and identify any irregular, extra or missing parts for diagnostic purposes. Karyotyping, the process of separating and classifying human chromosomes from a cell image, plays a crucial role in this diagnosis process.

However, accomplishing this work efficiently not only requires considerable manual efforts, domain expertise and experience, but also consumes a lot of time. Since 1980, with the motivation of lightening the load of cytogeneticists, automatic diagnosis systems for chromosome karyotyping and analysis have become a popular and important task.

With the development of CNNs, they have been utilized in medical image sector to deal with complicated features. CNN based models have been explored to analyze chromosome images. In this study, we consider to construct a new CNN based model to address the above issues.
