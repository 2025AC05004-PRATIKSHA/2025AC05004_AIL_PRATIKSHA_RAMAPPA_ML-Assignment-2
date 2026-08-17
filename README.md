# Credit Card Default Prediction

## a. Problem statement

This project develops and evaluates multiple machine learning classification models for predicting credit card default.

The implemented models are:

1. Logistic Regression
2. Decision Tree
3. k-Nearest Neighbors (kNN)
4. Naive Bayes
5. Random Forest (Ensemble)

The trained models are saved as `.pkl` files and are used by the Streamlit application for prediction and evaluation.

## b. Dataset description

The application uses the prepared credit card default test dataset.

The target variable is:

- `default` — indicates whether the customer defaulted.

The `test_data.csv` file is included in the project repository and is used for evaluating the saved machine learning models.

## c. Github Repository Link

https://github.com/2025AC05004-PRATIKSHA/2025AC05004_AIL_PRATIKSHA_RAMAPPA_ML-Assignment-2

## d. Models used

The following pre-trained models are included:

- Logistic Regression
- Decision Tree
- kNN
- Naive Bayes
- Random Forest (Ensemble)

All saved model files are stored inside the `model/` directory.

### Model Comparison

The models were evaluated using the following six metrics:

- Accuracy
- AUC
- Precision
- Recall
- F1 Score
- Matthews Correlation Coefficient (MCC)

| ML Model Name | Accuracy | AUC | Precision | Recall | F1 | MCC |
|---|---:|---:|---:|---:|---:|---:|
| Logistic Regression | 0.8088 | 0.7100 | 0.6923 | 0.2442 | 0.3610 | 0.3302 |
| Decision Tree | 0.8157 | 0.7398 | 0.6499 | 0.3610 | 0.4641 | 0.3866 |
| kNN | 0.7948 | 0.7041 | 0.5561 | 0.3587 | 0.4361 | 0.3292 |
| Naive Bayes | 0.2903 | 0.7240 | 0.2340 | 0.9714 | 0.3771 | 0.1034 |
| Random Forest (Ensemble) | 0.8155 | 0.7754 | 0.6580 | 0.3451 | 0.4528 | 0.3813 |

### Observations

| ML Model Name | Observation about model performance |
|---|---|
| Logistic Regression | Achieved the highest precision among the evaluated models, but its recall and F1 score were lower than Decision Tree and kNN. |
| Decision Tree | Achieved the highest accuracy, F1 score, and MCC among the evaluated models. |
| kNN | Achieved lower accuracy, AUC, precision, F1 score, and MCC than Decision Tree and Random Forest, while its recall was close to Decision Tree. |
| Naive Bayes | Achieved the highest recall, but its accuracy, precision, and MCC were substantially lower than the other models. |
| Random Forest (Ensemble) | Achieved the highest AUC among the evaluated models and provided strong accuracy, F1 score, and MCC performance. |

### Overall Winner for your dataset?

**Decision Tree**

Decision Tree achieved the highest Accuracy, F1 Score, and MCC among the evaluated models. Random Forest achieved the highest AUC, Logistic Regression achieved the highest Precision, and Naive Bayes achieved the highest Recall.
