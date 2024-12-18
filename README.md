# 🔍 Feature Selection in Machine Learning 🚀

🚀 Boost Model Performance by Selecting the Right Features!# Feature-Selection


## 📊 Overview

* Feature Selection is a crucial step in building robust and efficient machine learning models. It involves selecting the most relevant features from the dataset while discarding irrelevant or redundant ones.
* This repository showcases the process of feature selection applied to the **Human Activity Recognition with Smartphone Dataset** and **SECOND DATASET**.

## 🌐 Dataset Details:
* **Dataset Name**: Human Activity Recognition (HAR) with Smartphones
* **Features**: 561 numerical features
* **Target**: Human activity labels (e.g., Walking, Sitting, Standing)
* **Model Accuracy Before Feature Selection**: 98% (using all 561 features)

## By applying feature selection techniques, we aim to:
* Reduce dimensionality
* Improve computational efficiency
* Retain or improve model accuracy by removing noise

## ⚖️ Why Feature Selection?
### Key Benefits:

🎨 **Simpler Models**: Reduces model complexity and improves interpretability.

⏳ **Faster Computation**: Less data to process means quicker training.

❌ **Eliminates Noise**: Removes irrelevant or redundant features.

🔒 **Prevents Overfitting**: Focuses on relevant patterns, avoiding overfitting to noise.

## ⚙️ Feature Selection Workflow
### 🎯 Step-by-Step Sequence:

### 1. Split the Data (🔒 Avoid Data Leakage):
* Perform train-test split before any feature selection or preprocessing to ensure the test set remains unseen during feature selection. This avoids overestimating model performance.

### 2. Preprocess the Data:
  * Handle missing values, outliers, and standardize numerical features.
  * Apply One-Hot Encoding for categorical variables, if present.

### 3. Feature Selection (🔢 Types & Procedures):
  * Start with Filter Methods to remove highly correlated or irrelevant features.
  * Proceed with Wrapper Methods to evaluate subsets of features using model performance.
  * Finally, use Embedded Methods for feature importance scores directly from the model.

### 4. Train the Model with Selected Features:
  * Use only the retained features from the train set for model training.

### 5. Evaluate the Model:
  * Transform the test set using the same preprocessing pipeline and selected features.
  * Compare performance before and after feature selection.

## 🌐 Types of Feature Selection
### 1. ❌ Filter Methods (Univariate Selection):
* What? Rank features based on statistical tests and relationships with the target variable.
* Examples:
* Correlation Coefficient: For numerical features.
* Chi-Square Test: For categorical features and targets.
* ANOVA (F-Test): For numerical features with categorical targets.
* When? Initial step to eliminate obviously irrelevant features.

### 2. ⟳ Wrapper Methods (Model-Based Evaluation):
* What? Select subsets of features and evaluate performance iteratively.
* Examples:
* Recursive Feature Elimination (RFE): Systematically removes less important features based on model performance.
* Forward/Backward Feature Selection: Add/remove features incrementally.
* When? After filter methods to refine feature selection.

### 3. 🌳 Embedded Methods (Built-In Selection):
* What? Use models that have feature selection inherently built into them.
* Examples:
* Lasso Regression (L1 Regularization): Shrinks coefficients of irrelevant features to zero.
* Tree-Based Models: (e.g., Random Forest, XGBoost) provide feature importance scores.
* When? Final step for selecting features based on model insights.

## 🔍 Key Insights
* Feature Selection is Iterative: Combining filter, wrapper, and embedded methods provides the best results.
* Avoid Data Leakage: Always split data before preprocessing and feature selection.
* Tree-Based Models Shine: They naturally handle mixed data types and provide intuitive feature importance scores.

## 🔧 Technologies Used
* Python Libraries: sklearn, pandas, numpy, matplotlib, seaborn
* Models: Logistic Regression

### 📢 Contribute

Found this helpful? Feel free to open an issue or contribute improvements by submitting a pull request

### ✨ Future Work
* Explore deep learning feature selection techniques.
* Benchmark computational performance across large datasets.
