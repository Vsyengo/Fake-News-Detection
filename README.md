# Fake News Detection 

This project uses machine learning models to classify news articles as *real* or *fake* based on text structure and content features.

## What We Did
- Extracted features like article length, vocabulary richness, and keyword frequencies.
- Applied *Principal Component Analysis (PCA)* to reduce dimensionality.
- Trained and compared two models:
  - **Random Forest** (using `ranger`)
  - **Support Vector Machine (SVM)** both with linear and radial kernel

## Results
- Both models achieved over **83% accuracy** and about **70% Kappa** .
- **SVM** performed slightly better at detecting fake news.
- **Random Forest** offered better interpretability through variable importance.

## Files
- `*.Rmd`: Main analysis and model building
- `news_data.csv`: Datasets used
- `README.md`: Project summary

## Motivation
In an age of misinformation, building tools to automatically identify fake news is critical for protecting the public and supporting media literacy.

## Requirements
- R
- Libraries:
library(tidyverse)
library(dplyr)
library(tidytext)
library(SnowballC)
library(tm)
library(tidytext)
library(e1071)
library(caret)
library(ranger)
library(ggplot2)


