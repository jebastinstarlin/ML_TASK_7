# Credit Card Fraud Detection Using Machine Learning

## 1. Project Overview

Credit Card Fraud Detection is a Machine Learning project that identifies potentially fraudulent credit card transactions using a **Random Forest Classifier**. The model analyzes transaction data, classifies transactions as genuine or fraudulent, and evaluates its performance using various classification metrics.

## 2. Objectives

The primary objectives of this project are:

- To analyze credit card transaction data.
- To identify fraudulent and genuine transactions.
- To train a Machine Learning classification model.
- To evaluate model performance using classification metrics.
- To visualize the Confusion Matrix, ROC Curve, and feature importance.
- To identify detected and missed fraudulent transactions.

## 3. Technologies Used

The following technologies and libraries are used in this project:

- **Programming Language:** Python
- **Data Processing:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Development Environment:** Jupyter Notebook / Google Colab

## 4. Dataset

The project uses a credit card transaction dataset named `creditcard.csv`.

The target column is `Class`, which represents the transaction type:

- **0 – Genuine Transaction**
- **1 – Fraudulent Transaction**

**Note:** The dataset is not included in this repository. Download the dataset separately and update the file path in the notebook according to your environment.

## 5. Project Workflow

The project follows these steps:

1. **Data Loading:** Load the dataset using Pandas.
2. **Data Exploration:** Examine the dataset structure, data types, missing values, and class distribution.
3. **Data Preparation:** Separate the input features and target variable.
4. **Data Splitting:** Split the dataset into 80% training data and 20% testing data.
5. **Model Training:** Train a Random Forest Classifier with 100 decision trees.
6. **Prediction:** Predict whether transactions are genuine or fraudulent.
7. **Model Evaluation:** Evaluate performance using Precision, Recall, F1-Score, ROC-AUC, and the Classification Report.
8. **Fraud Analysis:** Analyze detected and missed fraudulent transactions.
9. **Feature Importance:** Identify and visualize the ten most important features.
10. **Visualization:** Generate the Confusion Matrix and ROC Curve.

## 6. Machine Learning Algorithm

### Random Forest Classifier

Random Forest is a supervised Machine Learning algorithm that combines multiple decision trees to make predictions. In this project, it is used to classify credit card transactions as genuine or fraudulent.

### Model Configuration

The Random Forest Classifier uses the following configuration:

- **Number of Estimators:** 100
- **Class Weight:** `balanced_subsample`
- **Random State:** 42
- **Test Size:** 20%
- **Parallel Processing:** `n_jobs=-1`

## 7. Evaluation Metrics

The model's performance is evaluated using the following metrics:

- **Precision:** Measures how many transactions predicted as fraudulent are actually fraudulent.
- **Recall:** Measures how many actual fraudulent transactions are correctly detected.
- **F1-Score:** Provides a balance between Precision and Recall.
- **ROC-AUC Score:** Measures the model's ability to distinguish between genuine and fraudulent transactions.
- **Confusion Matrix:** Displays the number of correct and incorrect predictions for each class.
- **Classification Report:** Provides Precision, Recall, F1-Score, and Support for each class.

## 8. Project Outputs

After executing the notebook, the following outputs are generated:

- Confusion Matrix visualization.
- Classification Report and evaluation metrics.
- Counts of detected and missed fraudulent transactions.
- Top 10 feature importance visualization.
- ROC Curve visualization.
- `actual_fraudulent_test_transactions.csv`, containing actual fraudulent transactions from the test dataset.

## 9. Future Enhancements

The project can be improved through the following enhancements:

- Compare Random Forest with other Machine Learning algorithms.
- Perform hyperparameter tuning to improve model performance.
- Apply cross-validation for more reliable evaluation.
- Optimize the prediction threshold to balance fraud detection and false alarms.
- Develop a web application for real-time fraud prediction.

## 10. Limitations

- **Imbalanced Dataset:** Fraudulent transactions are much less common than genuine transactions.
- **Accuracy Limitations:** Accuracy alone may not provide a reliable measure of fraud detection performance.
- **Data Dependency:** Model performance depends on dataset quality, selected features, and model configuration.
- **Educational Purpose:** The project is intended for educational purposes and is not a production-ready fraud prevention system.

## 11. Conclusion

The Credit Card Fraud Detection project demonstrates how Machine Learning can be used to identify potentially fraudulent financial transactions. By applying a Random Forest Classifier and evaluating its performance using multiple classification metrics, the project provides a practical introduction to fraud detection, data analysis, and predictive modeling.

The visualizations and fraud analysis further help users understand the model's predictions, identify important features, and evaluate its ability to detect fraudulent transactions.
