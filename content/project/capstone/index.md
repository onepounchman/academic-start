---
title: Examining the association between Socioeconomic Status(SES) and Air Pollution in Alameda County
summary: The goal is to learn about differential levels of air pollution exposure for different population groups
tags:
- Spatial Statistics
- Nearest Neighbor Gaussian Process 
- Enviromental Justice

date: "2020-12-3T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Spatial distribution of NO2
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

Air pollution is the release of pollutants into the air that is mainly due to human activities or natural processes, and it has become a severe consequence of industrialization and urbanization. It has been shown that air pollution is related to several health risks, such as stroke and aggravated respiratory disease. Moreover, it causes permanent damage to human’s nerve and other organs. According to the World Health Organization, 4.2 million deaths every year are caused by exposure to outdoor air pollution. Furthermore, several social studies have shown that racial minorities are considered to be more vulnerable to the process of urbanization and more susceptible to air pollution. 

Previous research has discussed environmental inequalities and environmental justice over the years. According to Hajat et al. (2015), ”Most North American studies have shown that areas where low socioeconomic status (SES) communities dwell experience higher concentrations of criteria air pollutants”. Therefore, conducting the association between SES and air quality is important in understanding the causes of disparities in health outcomes related to air pollution.  

Although previous research has shown environmental inequality in exposures to air pollution, most of them are based on air quality data from government-owned stationary monitors set in population centers, so they are considered to be not representative to assess local air pollutant characteristics among neighbourhoods. In this study, we used Aclima air pollution data (Aclima, Inc., San Francisco, CA), based on routine mobile monitoring with Google street view vehicles for time-integrate measurements at high spatial resolution. This innovative approach enables block-by-block measurements covering the whole Alameda county, which deliver up to 100,000 greater spatial resolution than traditional approaches and provide coverage at regional scales. Using Aclima’s high spatial resolution data, we conducted a granular analysis to assess the association between socioeconomic status (SES) and air pollutant exposure on road level.

Our primary outcome of interest will be NO2 because it has more spatial variation as the data visualization shows. The analysis goal is to examine the association between SES variables and NO2 air pollutant level. Linear regression model was built with log-transformed NO2 as outcome, with socio-economic related variables, income, education and employment status, adjusted for race/ethnicity and age. Correlation structure was added to the linear main model, adjusting for spatial correlation between NO2 measurements. We employed two approaches to estimate linear model parameters: Generalized estimating equation (GEE) and Gaussian Bayesian spatial regression models using Nearest Neighbor Gaussian Processes (NNGP).
