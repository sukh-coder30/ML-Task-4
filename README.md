# ML-Task-4
This project demonstrates how to train and evaluate a Logistic Regression classifier on the Breast Cancer Wisconsin (Diagnostic) dataset. It also visualizes the sigmoid function to illustrate how model logits are converted into probabilities.

📋 Overview
The Breast Cancer dataset consists of measurements from digitized images of fine needle aspirate (FNA) of breast masses. Each observation describes properties of cell nuclei, and the task is to classify tumors as:

Malignant (cancerous)

Benign (non-cancerous)

This project includes:

 Data loading and preprocessing
 Logistic Regression training
 Probability calculation using the sigmoid function
 Threshold tuning for classification
 Visualization of the sigmoid transformation

Dataset
Source: UCI Machine Learning Repository
File: CSV format containing columns:

id: Sample ID

diagnosis: M (malignant) or B (benign)

30 numeric features describing cell characteristics

Before modeling:

diagnosis is mapped to numeric labels (M=0, B=1)

id column is removed

⚙️ Workflow
Data Preparation

Load CSV with Pandas

Encode target labels

Scale features with StandardScaler

Model Training

Logistic Regression is fit on training data

Probability Prediction

Raw logits are extracted using decision_function()

Sigmoid function applied to compute probabilities

Threshold Tuning

Predictions are classified using custom thresholds (e.g., 0.3, 0.5, 0.7)

Performance evaluated with confusion matrix and classification report

Visualization

Sigmoid curve plotted to show transformation of logits into probabilities

Load data

Train model

Evaluate predictions

Generate visualizations

Adjust the threshold as needed to balance sensitivity and specificit
