# **Breast Cancer Diagnostic Analysis and Prediction**

This repository contains an end-to-end project on breast cancer diagnosis prediction based on features derived from the publication ["Nuclear feature extraction for breast tumor diagnosis"](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/1905/1/Nuclear-feature-extraction-for-breast-tumor-diagnosis/10.1117/12.148698.short?SSO=1).

## **Project Structure**:

```
Breast_cancer_prediction
├── data/
│   ├── data.csv
│   ├── data_label_encoded.csv
│   └── data_pca_10.csv
├── model/
│   └── logistic_regression_best_model.pkl
├── notebooks/
│   ├── data_preprocessing.ipynb
│   └── classification-model.ipynb
└── README.md
```


### **Data**:
- `data.csv`: Original dataset.
- `data_label_encoded.csv`: Dataset with the target column 'diagnosis' encoded into numerical format.
- `data_pca_10.csv`: Dataset transformed using PCA retaining 10 principal components.

### **Model**:
- `logistic_regression_best_model.pkl`: Trained and optimized Logistic Regression model for predicting breast cancer diagnosis.

### **Notebooks**:
- `data_preprocessing.ipynb`: Jupyter notebook detailing the steps taken for data exploration, cleaning, and preprocessing.
- `classification-model.ipynb`: Jupyter notebook covering the machine learning modeling and evaluation steps.

## Data Exploration:

- The dataset contained 569 records and 32 features, which included an 'id' column, a target column 'diagnosis', and 30 numerical features describing the characteristics of cell nuclei.
- There were two classes in the target variable: Benign (B) and Malignant (M).
- The data was relatively clean with no missing values.

## Exploratory Data Analysis (EDA):

- Univariate analysis revealed the distribution of each feature, providing insights into their nature.
- Pair plots showed relationships between features and their impact on the diagnosis.
- The correlation matrix identified strongly correlated features. Some features had a high degree of correlation, suggesting potential multicollinearity.

## Data Preprocessing:

- The target column 'diagnosis' was encoded into numerical format (M:1, B:0).
- Features were standardized to have a mean of 0 and a standard deviation of 1.
- PCA was applied to reduce dimensionality, retaining 10 principal components that captured most of the variance in the data.

## Modeling:

- Several classifiers, including Logistic Regression, Random Forest, Gradient Boosting, and SVM, were trained and evaluated.
- Logistic Regression was chosen for further optimization.
- Hyperparameter tuning was conducted on Logistic Regression using GridSearchCV.
- The tuned Logistic Regression model performed well, with an AUC score close to 0.99, suggesting a strong predictive capability.

## **Dataset**:

https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic

