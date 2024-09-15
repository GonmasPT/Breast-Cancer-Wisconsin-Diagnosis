# Breast Cancer Wisconsin Diagnosis

This repository focuses on the classification of breast cancer tumors as either malignant or benign using the Breast Cancer Wisconsin (Diagnostic) Dataset from Kaggle. The goal of the project is to build machine learning models that can accurately predict whether a tumor is malignant (cancerous) or benign (non-cancerous), based on the characteristics of the tumor.

### Project Overview

The project is structured in three main stages:

<ol>
<li>Data Visualization</li>

<li>Feature Selection</li>

<li>Model Development</li>
</ol>

### 1. Data Visualization

To begin, I explore the dataset through a series of visualizations to understand the distributions, relationships, and patterns in the data. Key steps include:

<ul>
<li>Examining the class distribution of the target variable (malignant vs. benign).</li>

<li>Visualizing individual features using box plots and swarm plots to identify trends and outliers.</li>

<li>Studying feature relationships and correlations using heatmaps to detect highly correlated features and gain insights into feature interactions.</li>
</ul>

### 2. Feature Selection

After visualizing the data, I proceed to reduce dimensionality by applying feature selection techniques:

<ul>
<li>Manual Selection: Based on a correlation heatmap, highly correlated features were manually removed to avoid multicollinearity. By removing one feature from each highly correlated pair, I ensured that the model does not rely on redundant information, improving its interpretability and performance.</li>

<li>RFECV: Recursive Feature Elimination with Cross-Validation was applied to automatically rank and select the most important features. This method recursively removes the least important features and uses cross-validation to evaluate model performance. The optimal number of features was determined based on the model's performance, ensuring that only the most relevant features are kept for training the model.</li>
</ul>

### 3. Model Development

Once the data is prepared, I train several machine learning models to classify tumors as malignant or benign. The models include:

<ul>
<li>Random Forest</li>

<li>Logistic Regression</li>

<li>K-Nearest Neighbors (KNN)</li>

<li>Support Vector Machines (SVM)</li>

<li>XGBoost</li>
</ul>

I applied cross-validation to evaluate the performance of each model, using recall as the primary metric throughout the notebook. Recall was chosen to prioritize minimizing false negatives, particularly important for this classification task. After identifying the best-performing model, I further assessed its performance using additional metrics, including accuracy, precision, and F1-score, for a more comprehensive evaluation.

### Dataset

The dataset used for this project is the Breast Cancer Wisconsin (Diagnostic) Dataset, which contains 30 features representing various measurements of cell nuclei present in breast cancer biopsies. The target variable is binary (malignant or benign).

<ul>
<li>Rows: 569</li>
  
<li>Features: 32 (e.g., radius_mean, texture_mean, perimeter_mean, area_mean, smoothness_mean)</li>

<li>Target: Binary (malignant = 1, benign = 0)</li>
</ul>

### Conclusion

This project demonstrates the process of building a classification model from raw data to final predictions. By combining data visualization, feature selection, and machine learning techniques, I aimed to improve model performance and gain insights into the most significant features contributing to tumor classification.
