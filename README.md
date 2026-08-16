# Credit Card Default Prediction

## 1. Project Overview

This project develops and evaluates multiple machine learning classification
models for predicting credit card default.

The implemented models are:

1. Logistic Regression
2. Decision Tree
3. k-Nearest Neighbors (kNN)
4. Naive Bayes
5. Random Forest

The trained models are saved as `.pkl` files and are used by the Streamlit
application for prediction and evaluation.


## 2. Dataset

The application uses the prepared credit card default test dataset.

The target variable is:

- `default` — indicates whether the customer defaulted.

The `test_data.csv` file is included in the project repository and is used
for evaluating the saved machine learning models.


## 3. Machine Learning Models

The following pre-trained models are included:

- Logistic Regression
- Decision Tree
- kNN
- Naive Bayes
- Random Forest

All saved model files are stored inside the `model/` directory.


## 4. Model Evaluation

The models were evaluated using the following six metrics:

- Accuracy
- AUC
- Precision
- Recall
- F1 Score
- Matthews Correlation Coefficient (MCC)

### Model Comparison

| Model               | Accuracy   | AUC    | Precision   | Recall   | F1 Score   | MCC    |
|:--------------------|:-----------|:-------|:------------|:---------|:-----------|:-------|
| Logistic Regression | 0.8088     | 0.7100 | 0.6923      | 0.2442   | 0.3610     | 0.3302 |
| Decision Tree       | 0.8157     | 0.7398 | 0.6499      | 0.3610   | 0.4641     | 0.3866 |
| kNN                 | 0.7948     | 0.7041 | 0.5561      | 0.3587   | 0.4361     | 0.3292 |
| Naive Bayes         | 0.2903     | 0.7240 | 0.2340      | 0.9714   | 0.3771     | 0.1034 |
| Random Forest       | 0.8155     | 0.7754 | 0.6580      | 0.3451   | 0.4528     | 0.3813 |

## 5. Observations

The latest evaluation results show:

- **Accuracy:** Decision Tree achieved the highest accuracy.
- **AUC:** Random Forest achieved the highest AUC.
- **Precision:** Logistic Regression achieved the highest precision.
- **Recall:** Naive Bayes achieved the highest recall.
- **F1 Score:** Decision Tree achieved the highest F1 score.
- **MCC:** Decision Tree achieved the highest MCC.

Naive Bayes achieves the highest recall, but its overall accuracy,
precision and MCC are substantially lower than the other models.

Random Forest provides the strongest AUC performance among the evaluated
models, while Decision Tree provides the highest accuracy and F1 score.


## 6. Streamlit Application

The project includes a Streamlit application in `app.py`.

The application allows the user to:

- Select a pre-trained machine learning model.
- Upload the test CSV file.
- Generate predictions.
- View Accuracy, AUC, Precision, Recall, F1 Score and MCC.
- View the confusion matrix.
- View the classification report.
- Download prediction results as a CSV file.


## 7. Project Structure

ML_Assignment_2_App/
├── app.py
├── requirements.txt
├── test_data.csv
├── README.md
└── model/
    ├── logistic_regression.pkl
    ├── decision_tree.pkl
    ├── knn.pkl
    ├── naive_bayes.pkl
    └── random_forest.pkl


## 8. Requirements

The required Python libraries are listed in `requirements.txt`.


## 9. Running the Application

Install the required dependencies:

`pip install -r requirements.txt`

Run the Streamlit application:

`streamlit run app.py`

The application will open in a browser and allow the user to select a model
and upload the test CSV file.


## 10. Deployment

The application is intended to be deployed using Streamlit Community Cloud.

The deployed application should use this GitHub repository and the `master`
branch.


## 11. Reproducibility

The model comparison table in this README is generated from the current
saved `.pkl` model files and `test_data.csv`.

To regenerate the results, load the five saved models, evaluate them on the
test dataset using the six required metrics, and regenerate this README.
