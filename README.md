## Colon Cancer Prediction Model from Multiple Datasets

### Introduction

Colorectal cancer is the third leading cause of cancer-related deaths in the United States, but it has a high survival rate if detected early. This project aims to build a machine learning model that can accurately predict the type of colon cancer using data from two separate datasets.

### Data Preprocessing

The first step in building the model was to preprocess the data. This involved:

- **Initial analysis**: We analyzed each dataset to understand the distribution of features and identify potential correlations.
- **Merging datasets**: Since the datasets had different columns, we merged them using the `concat()` function in Pandas.
- **Treating outliers**: We used the KNN imputer to fill in missing values and treat outliers.

### 3. Model Building

**3.1 Model Selection**

Multiple machine learning models were evaluated for the task of colon cancer type prediction, including:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree Classifier
- Ensemble Techniques (Random Forest, Gradient Boosting Classifier)
- XGBoost
### Model Optimization

We optimized the models using the following techniques:

- **Feature engineering**: We derived new features by combining existing features, such as creating a "health risk score" based on smoking history and family history of cancer.
- **Hyperparameter tuning**: We used grid search to find the best hyperparameters for each model.

### Evaluation

We evaluated the models using the following metrics:

- **Accuracy**: The percentage of correct predictions.
- **Precision**: The percentage of predicted positives that are actually positive.
- **Recall**: The percentage of actual positives that are predicted positive.
- **F1-score**: The harmonic mean of precision and recall.

### Results

The Decision Tree Classifier outperformed the Logistic Regression model on all metrics. The best results were:

| Metric | Score |
|---|---|
| Accuracy | 81.25% |
| Precision | 81.50% |
| Recall | 81.25% |
| F1-score | 81.23% |

### Conclusion

We successfully built a machine learning model that can predict the type of colon cancer with high accuracy. The model can be used by healthcare professionals to assist in early detection and accurate prediction of colon cancer type.

### Documentation

The full code for this project is available on GitHub and Google Colab.

### Screenshots
**Data Preprocessing**
![Screenshot 2024-11-11 152529](https://github.com/user-attachments/assets/a9ffaf10-d84e-467c-910a-877afdcec89f)

![Screenshot 2024-11-11 152501](https://github.com/user-attachments/assets/e74e9519-837f-4838-b2b5-0fba945c844d)
**evaluation**
![Screenshot 2024-11-11 152401](https://github.com/user-attachments/assets/1e1584c8-86ca-4f78-8823-3c0cd3c419f5)

