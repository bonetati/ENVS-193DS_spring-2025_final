# ENVS 193DS, Final Project Problem 3  
**Spring 2025**

## General information  
This dataset is from:  
Stojanovic, Dejan; Owens, Grace; Young, Claudia M.; Alves, Felipe; Heinsohn, Robert (2021). *Do nest boxes breed the target species or its competitors? A case study of a critically endangered bird.* Dryad. https://doi.org/10.5061/dryad.83bk3j9sb  

The published paper is:  
Stojanovic, D., Owens, G., Young, C. M., Alves, F., & Heinsohn, R. (2021). *Do nest boxes breed the target species or its competitors? A case study of a critically endangered bird.* Restoration Ecology, 29(1), e13319. https://doi.org/10.1111/rec.13319  

This repository demonstrates fitting generalized linear models with categorical and continuous predictors, model selection using AIC, and visualizing model predictions for a binary response variable (nest box occupancy).

## Data and file overview
```{r file-structure}
list.files(path = ".", recursive = TRUE)
---

## Packages  
```r
library(tidyverse)   # data wrangling and plotting  
library(janitor)     # cleaning column names  
library(here)        # file path consistency  
library(DHARMa)      # model diagnostics  
library(MuMIn)       # model selection (AIC)  
library(ggeffects)   # generating predicted values and confidence intervals  
