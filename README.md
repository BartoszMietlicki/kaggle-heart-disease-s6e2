# Kaggle Playground S6E2 — Heart Disease Prediction

This repository contains my solution notebook for **Kaggle Playground Series (Season 6, Episode 2)**.
The goal is to predict the probability of the positive class for the competition test set and generate a valid submission.

**Competition:** https://www.kaggle.com/competitions/playground-series-s6e2 

**My Kaggle notebook:** https://www.kaggle.com/code/bartekmietlicki/bm-heartdisease-s6e2-k

## What was done
Three model families were evaluated using the same cross-validation strategy (**StratifiedKFold**) and the same metric (**ROC AUC**) to ensure a fair comparison:

- **Logistic Regression** (baseline)
- **XGBoost** (best CV ROC AUC, selected for final training)
- **TabNet** (neural network for tabular data)

The final model is trained on the full training set and used to generate probabilities for the test set.

## Notes on running
- **Recommended:** run on **Kaggle Notebooks** using the competition dataset input.
- Running in **Google Colab** is possible, but it requires a **personal Kaggle API token** added to Colab *Secrets* and downloading the competition data via the Kaggle API.
- The notebook includes small environment-specific sections (Kaggle vs Colab) for data importing.
