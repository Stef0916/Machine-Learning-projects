# Diabetes Detection using Different Classifaction Methods and Artificial Neural Network

The objective of the project is to build a reliable and robust ML classification algorithm in order to predict whether or not a patient has diabetes, based in given features/diagnostic measurements. It includes data preprocessing, feature selection, and model building and evaluation.

<u>**`Some important considerations`:**</u>

- Only female patients are considered with at least 21 years old of Prima Indian hertiage.

- The dataset was taken from the publication [Using the ADAP Learning Algorithm to Forecast the Onset of Diabetes Mellitus](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2245318/). The original publication can be found in the References folder within this project.
- Dataset: https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

**NOTE**: This dataset has a controversial background, as highlighted in this [journal](https://www.journals.uchicago.edu/doi/full/10.1086/693853) (and can be found in the `References` folder within this project). I am firmly against any discriminatory behaviors based on ethnicity or gender. My use of this dataset is purely for educational purposes, as it presents certain challenges I wish to overcome, such as a big cluster of missing data within its features. It's crucial to approach ML/AI topics with care and responsibility.

## Project Structure

```plaintext
/diabetes-prediction_Classification_ANN
|-- data/
|   |-- diabetes_clean_scaled_categorical_pregnancies.csv  # Scaled data with categorical pregnancies
|   |-- diabetes_clean_scaled.csv  # Scaled version of the original dataset
|   |-- diabetes.csv  # Raw diabetes dataset
|-- model/
|   |-- diabetes-lightgbm.pkl  # LightGBM trained model for diabetes prediction with pycaret
|-- notebooks/
|   |-- data_preprocessing-1.ipynb  # Notebook detailing preprocessing of data
|   |-- pregnancies-categorical-or-numerical-2.ipynb  # Exploration on treating pregnancies as categorical or numerical
|   |-- feature-selection-3.ipynb  # Feature selection strategies and findings
|   |-- classification-model-4.ipynb  # Notebook detailing the building and evaluation of the classification model
|   |-- Diabtetes-detection-pycaret-5.ipynb  # Model building and detection using PyCaret
|-- references/
|   |-- procascamc00018-0276.pdf  # Reference paper related to the dataset
|   |-- radin-2017-digital-natives-how-medical-and-indigenous-histories-matter-for-big-data.pdf  # Reference paper on the importance of medical and indigenous histories for big data
|-- README.md  # This file, detailing the project structure and overview
```


## Data

The `data` directory contains three datasets:
- `diabetes.csv`: This is the raw dataset containing information about various patients and whether they have diabetes.
- `diabetes_clean_scaled.csv`: This is the scaled version of the original dataset, optimized for machine learning models.
- `diabetes_clean_scaled_categorical_pregnancies.csv`: This dataset treats the pregnancies feature as a categorical variable.

## Model

The trained LightGBM model used for predicting diabetes is stored as `diabetes-lightgbm.pkl`.

## Notebooks

The notebooks provide a step-by-step walkthrough of the project:
1. `data_preprocessing-1.ipynb`: Details the preprocessing steps applied to the raw data.
2. `pregnancies-categorical-or-numerical-2.ipynb`: Explores the decision of treating the pregnancies feature as either categorical or numerical.
3. `feature-selection-3.ipynb`: Discusses feature selection strategies and their outcomes.
4. `classification-model-4.ipynb`: Describes the building, training, and evaluation of the classification model.
5. `Diabtetes-detection-pycaret-5.ipynb`: Demonstrates model building and evaluation using the PyCaret library.

## Data Reference

https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

## References

This section contains academic and other authoritative references that have been instrumental in guiding the project:
- `procascamc00018-0276.pdf`: A paper that provides insights into the dataset or methodology used.
- `radin-2017-digital-natives-how-medical-and-indigenous-histories-matter-for-big-data.pdf`: This paper discusses the importance of considering medical and indigenous histories when working with big data.