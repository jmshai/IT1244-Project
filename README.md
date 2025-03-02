# Cancer Classification Project

## Overview
This project focuses on classifying cancer stages using machine learning techniques. The dataset contains multiple features related to patient health, and the goal is to build a model that accurately differentiates between different stages of cancer.

## Dataset
- **Dataset:** `Train_Set.csv`
- **Features:** Approximately 350
- **Target Variable (`class_label`)** includes:
  - 🟢 **Healthy**
  - 🟡 **Screening stage cancer**
  - 🔵 **Early stage cancer**
  - 🟠 **Mid stage cancer**
  - 🔴 **Late stage cancer**

**Data Imbalance:** Many samples belong to early-stage cancer, with fewer representing healthy individuals.

## Methodology
### 1. Data Preprocessing
- Load and explore the dataset.
- Normalize feature values.
- Address class imbalance by combining certain categories for classification.

### 2. Multi-Step Classification Approach
#### First Classifier:
Groups data into broad categories:
- **Healthy + Screening**
- **Late-stage cancer**
- **Early-stage cancer**
- **Mid-stage cancer**

#### Second Classifier:
Further differentiates between closely related categories (e.g., healthy vs. screening-stage cancer).

### 3. Machine Learning Models
- 🌲 **Random Forest Classifier**
- ⚡ **XGBoost Classifier**
- 🔍 **Hyperparameter tuning using GridSearchCV**
- 📊 **Performance evaluation with classification reports & confusion matrices**

## Requirements
To run this project, install the necessary Python libraries:
```bash
pip install numpy pandas scikit-learn matplotlib xgboost
```

## Execution Steps
1. Load the dataset (`Train_Set.csv`).
2. Perform exploratory data analysis.
3. Preprocess and normalize the data.
4. Train the models and evaluate performance.
5. Fine-tune hyperparameters for better accuracy.

## References
- *Application of Support Vector Machine Algorithm for Early Differential Diagnosis of Prostate Cancer*
- *Breast Cancer Diagnosis Based on K-Nearest Neighbors: A Review*

## Limitations
- ❗ Models may struggle with high-dimensional and multi-class data.
- ⚠️ Performance depends on data quality and preprocessing techniques.

## Conclusion
This project employs a structured, multi-step classification approach to improve cancer diagnosis accuracy. By leveraging machine learning techniques, we aim to enhance early detection and contribute to cancer research advancements.
