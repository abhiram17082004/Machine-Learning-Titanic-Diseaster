# Titanic Survival Prediction using Logistic Regression

## Overview

This project predicts whether a passenger survived the Titanic disaster using Machine Learning techniques. The project uses the Titanic dataset from Kaggle and applies data preprocessing, feature engineering, visualization, and Logistic Regression for classification.

The notebook was developed using Google Colab and Python libraries for data analysis and machine learning.

---

## Open in Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/abhiram17082004/Machine-Learning-Titanic-Diseaster/blob/main/TitanicDiseaster.ipynb)

---

## GitHub Repository

Repository Link:  
https://github.com/abhiram17082004/Machine-Learning-Titanic-Diseaster

---

## Dataset

The dataset used in this project is from the Kaggle Titanic Competition.

Dataset Link:  
https://www.kaggle.com/c/titanic

Direct Dataset Files:
- https://www.kaggle.com/c/titanic/data?select=train.csv
- https://www.kaggle.com/c/titanic/data?select=test.csv

The dataset contains passenger information such as:
- Passenger Class
- Gender
- Age
- Fare
- Family Details
- Embarkation Port

Target Variable:
- `0` → Did Not Survive
- `1` → Survived

---

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Machine Learning Model

### Logistic Regression

The Logistic Regression algorithm was used to classify whether a passenger survived or not based on passenger attributes.

---

## Project Workflow

1. Import Libraries
2. Load Titanic Dataset
3. Handle Missing Values
4. Age Imputation using Passenger Class
5. Data Visualization using Heatmaps
6. Feature Engineering
7. Convert Categorical Data using `get_dummies()`
8. Train-Test Split
9. Train Logistic Regression Model
10. Generate Predictions
11. Evaluate Model Performance

---

## Features Used

| Feature | Description |
|---|---|
| Pclass | Passenger Class |
| Sex | Gender |
| Age | Passenger Age |
| SibSp | Number of Siblings/Spouses |
| Parch | Number of Parents/Children |
| Fare | Ticket Fare |
| Embarked | Boarding Port |

---

## Data Preprocessing

The following preprocessing steps were performed:

- Filled missing Age values using Passenger Class averages
- Removed Cabin column due to excessive missing values
- Dropped unnecessary columns:
  - Name
  - Ticket
- Converted categorical variables into numerical format using one-hot encoding

---

## Sample Model Code

```python
from sklearn.linear_model import LogisticRegression

logmodel = LogisticRegression(max_iter=1000)

logmodel.fit(X_train, y_train)

predictions = logmodel.predict(X_test)
```

---

## Model Accuracy

The Logistic Regression model achieved an accuracy of approximately:

```text
81.27%
```

---

## Confusion Matrix

```text
[[150  13]
 [ 37  67]]
```

---

## Classification Report

| Metric | Class 0 | Class 1 |
|---|---|---|
| Precision | 0.80 | 0.84 |
| Recall | 0.92 | 0.64 |
| F1-Score | 0.86 | 0.73 |

Overall Accuracy: **81%**

---

## Project Structure

```text
Machine-Learning-Titanic-Diseaster/
│
├── TitanicDiseaster.ipynb
├── README.md
├── train.csv
├── test.csv
└── images/
```

---

## How to Run the Project

1. Open the notebook in Google Colab
2. Upload the Titanic dataset files
3. Run all notebook cells sequentially
4. The model will train and generate predictions

---

## Future Improvements

- Hyperparameter tuning
- Feature scaling
- Try advanced algorithms like Random Forest and XGBoost
- Deploy the model using Streamlit or Flask
- Improve prediction accuracy

---

## Conclusion

This project demonstrates a complete Machine Learning workflow including:
- Data preprocessing
- Missing value handling
- Feature engineering
- Logistic Regression classification
- Model evaluation using accuracy score, confusion matrix, and classification report

The project provides practical experience in supervised machine learning and classification problems using real-world data.

---

## Author

Abhiram
