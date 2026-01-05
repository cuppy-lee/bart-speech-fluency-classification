# Speech Fluency Classification using BART 

## Overview
This project uses a **Bayesian Additive Regression Trees (BART)** model to classify speech fluency from audio samples.
It also analyzes **Random Forest** and **XGBoost** models for comparison and explores **quantification of uncertainty** in predictions.

---

## Dataset

This project uses the **ArL2Eng dataset** published by **Nature** and can be found [here](https://rdcu.be/eXzUY). 
The dataset has two goals:
1. Predict English fluency among speakers and learners of Arab accents.
2. Identify Arabic accents from spoken L2 English speech.

**Note:** The speech corpus itself is not included in this repository. However, the extracted features are provided in the CSV files.

---

## Methodology

The repository includes two main notebooks:
1. `feature_extraction.ipynb`: Extracts speech features (MFCCs, F0, RMS) from audio files for use in model training.
2. `accent_classification.ipynb`: Performs speech fluency classification using BART, Random Forest, and XGBoost. Evaluates model performance and uncertainty quantification.  

*Additional experiment*: A brief section in `accent_classification.ipynb` tests BART and Random Forest models on Arabic accent classification, which was not the main focus of this project.

---

## How to Run

### Feature Extraction
There are two options:

1. Download the speech corpus from the source and extract features by running `feature_extraction.ipynb`.
2. Use the provided CSV files containing the extracted features.

### Model Training and Evaluation
1. Store the extracted features in CSV files in the same folder as `accent_classification.ipynb`.
2. Open and run `accent_classification.ipynb` to train the models and evaluate results.
