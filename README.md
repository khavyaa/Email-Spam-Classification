# Email-Spam-Classification
"Email spam classification project employing Naive Bayes classifiers for accurate email filtering."

This project explores the effectiveness of different Naive Bayes classifiers for email spam classification. We compare the performance of Gaussian, Multinomial, and Bernoulli Naive Bayes classifiers using various metrics and evaluate their suitability for the task of spam detection.

## Overview

Email spam classification is a common application of machine learning techniques, particularly Naive Bayes classifiers. In this project, we use a dataset of labeled emails (spam or non-spam) to train and evaluate three types of Naive Bayes classifiers.

## Dataset

The dataset used for this project consists of a collection of labeled emails, where each email is labeled as either spam or non-spam (ham). It is pre-processed and split into training and testing sets.

## Methodology

### 1. Data Preprocessing

- Tokenization: Convert raw email text into a bag-of-words representation.
- Feature Extraction: Use TF-IDF (Term Frequency-Inverse Document Frequency) to extract features from the text data.

### 2. Model Training

- **Gaussian Naive Bayes**:
  - Suitable for continuous features assuming a Gaussian distribution.
  - Training on numerical features extracted using TF-IDF.

- **Multinomial Naive Bayes**:
  - Appropriate for discrete features like word counts in text data.
  - Training on TF-IDF vectors representing word frequencies.

- **Bernoulli Naive Bayes**:
  - Designed for binary feature vectors (0s and 1s), suitable for presence/absence features.
  - Training on binarized TF-IDF vectors.

### 3. Model Evaluation

We evaluate the performance of each classifier using the following metrics:

- Accuracy
- Precision
- Confusion Matrix

## Results

The results of the experiment are as follows:

- **Gaussian Naive Bayes**:
  - Accuracy: 85.40%
  - Precision: 0.46

- **Multinomial Naive Bayes**:
  - Accuracy: 97.20%
  - Precision: 1.00

- **Bernoulli Naive Bayes**:
  - Accuracy: 98.26%
  - Precision: 0.99

## Conclusion

Based on the evaluation metrics, we conclude that Multinomial Naive Bayes is the most effective Naive Bayes classifier for email spam classification in this scenario. Further optimization and experimentation can be done to improve the results.

---
