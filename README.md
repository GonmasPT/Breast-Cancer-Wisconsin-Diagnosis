# Breast Cancer Wisconsin Diagnosis

This repository focuses on the classification of breast cancer tumors as either malignant or benign using the Breast Cancer Wisconsin (Diagnostic) Dataset from Kaggle. The goal of the project is to build machine learning models that can accurately predict whether a tumor is malignant (cancerous) or benign (non-cancerous), based on the characteristics of the tumor.

### Project Overview

The project is structured in three main stages:

<ol>
<li>Data Visualization</li>

<li>Feature Selection and Feature Extraction</li>

<li>Machine Learning Model Training</li>
</ol>

### 1. Data Visualization

To begin, I explore the dataset through a series of visualizations to understand the distributions, relationships, and patterns in the data. Key steps include:

<ul>
<li>Examining the class distribution of the target variable (malignant vs. benign).</li>

<li>Visualizing individual features using box plots, swarm plots, and histograms to identify trends and outliers.</li>

<li>Studying feature relationships and correlations using scatter plots and heatmaps to detect highly correlated features and gain insights into feature interactions.</li>
</ul>

### 2. Feature Selection and Feature Extraction

After visualizing the data, I proceed to reduce dimensionality by applying both feature selection and feature extraction techniques:

<ul>
<li>Feature Selection: Identifying the most relevant features that contribute to the classification task. I evaluate feature importance using methods like correlation analysis and statistical tests, removing redundant or irrelevant features.</li>

<li>Feature Extraction: Techniques such as Principal Component Analysis (PCA) are used to transform the feature set into a lower-dimensional space, capturing the most significant variance in the data while reducing noise and complexity.</li>
</ul>

### 3. Machine Learning Model Training

Once the data is prepared, I train several machine learning models to classify tumors as malignant or benign. The models include:

<ul>
<li>K-Nearest Neighbors (KNN)</li>

<li>Support Vector Machines (SVM)</li>

<li>Random Forest</li>

<li>Logistic Regression</li>
</ul>

I use cross-validation to assess model performance and fine-tune hyperparameters. The evaluation metrics include accuracy, precision, recall, F1-score, and the confusion matrix to ensure a comprehensive understanding of model effectiveness, especially in the presence of an imbalanced dataset.

### Dataset

The dataset used for this project is the Breast Cancer Wisconsin (Diagnostic) Dataset, which contains 30 features representing various measurements of cell nuclei present in breast cancer biopsies. The target variable is binary (malignant or benign).

<ul>
<li>Rows: 569</li>
  
<li>Features: 32 (e.g., radius_mean, texture_mean, perimeter_mean, area_mean, smoothness_mean)</li>

<li>Target: Binary (malignant = 1, benign = 0)</li>
</ul>

### Conclusion

This project demonstrates the process of building a classification model from raw data to final predictions. By combining data visualization, feature selection, and machine learning techniques, I aimed to improve model performance and gain insights into the most significant features contributing to tumor classification.
