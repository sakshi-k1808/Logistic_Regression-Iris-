# Logistic_Regression-Iris-

## Libraries Used

* **Pandas:** For data manipulation and analysis (using DataFrames).
* **Seaborn:** For loading the Iris dataset.
* **Scikit-learn:**
    * `train_test_split` for splitting data into training and testing sets.
    * `LogisticRegression` for the Logistic Regression model.
    * Metrics (`confusion_matrix`, `accuracy_score`, `recall_score`, `precision_score`, `classification_report`, `f1_score`) for evaluating the model's performance.
* **Warnings:** To suppress warnings.

## Data

The Iris dataset is loaded directly using Seaborn's `load_dataset` function.  It contains measurements (sepal length, sepal width, petal length, petal width) for three species of Iris: setosa, versicolor, and virginica.

## Data Exploration

1.  The notebook displays the first few and last few rows of the dataset using `df.head()` and `df.tail()`.
2.  `df.info()` is used to show information about the data types and null values.
3.  `df.describe()` provides descriptive statistics of the numerical features.

## Model Training and Evaluation

1.  **Data Separation:** The dataset is divided into features (X) and target variable (y), where X contains the measurements and y contains the species labels.
2.  **Train-Test Split:** The data is split into training and testing sets using `train_test_split`.
3.  **Model Training:** A `LogisticRegression` model is initialized and trained on the training data.
4.  **Prediction:** The trained model is used to predict the species for the test data.
5.  **Evaluation:** Several metrics are used to evaluate the model's performance:
    * **Confusion Matrix:** Shows the counts of correct and incorrect predictions for each class.
    * **Recall:** The ability of the model to correctly identify instances of each class.
    * **Precision:** The ability of the model to avoid misclassifying an instance as a certain class.
    * **F1-score:** The harmonic mean of precision and recall.
    * **Classification Report:** Provides a comprehensive summary of precision, recall, F1-score, and support for each class.
    * **Accuracy:** Overall accuracy of the model.

## Summary

This notebook demonstrates a complete workflow for building and evaluating a Logistic Regression model on the Iris dataset. It covers data loading, exploration, preprocessing (splitting), model training, prediction, and thorough performance evaluation.  The results showcase the effectiveness of Logistic Regression for this multi-class classification problem.
