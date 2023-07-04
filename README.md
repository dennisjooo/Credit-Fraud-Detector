# Comparative Analysis of Fraud Detection Models

**Created by:**

- Dennis Jonathan
- Sergio Gracia Darrell

Done as a final exam for Design and Analysis for Data Science course, Universitas Prasetiya Mulya

## Brief Background

Payment card fraud is an ongoing major issue in the financial industry, causing substantial financial losses projected to reach 40 billion dollars in 2027. As the industry grows, detecting fraud patterns becomes inherently difficult, almost impossible to detect manually.

Nowadays, the design of payment card fraud detection techniques rely on the use of unsupervised machine learning studying an imbalanced dataset uncovering patterns and outliers.

## Dataset

Taken from [Lopez-Rojas's Paysim dataset](https://www.kaggle.com/datasets/ealaxi/paysim1). It contains 6 million transactions, with 11 features. The dataset is highly imbalanced, with only 0.13% of the transactions being fraudulent.

## Brief Results

We compared three methods, namely:

- K-Means Clustering
- Gaussian Mixture
- AutoEncoder

The AutoEncoder method outperformed the other two methods with an AUC of 0.93. The reconstruction threshold was tuned to maximize the F1 score, which was 0.86.

The reason why the model was tuned the threshold to maximize the F1 score was because although it is important to minimise the number of false negatives, flagging a lot of transactions as fraudulent would be a hassle for the customers.
