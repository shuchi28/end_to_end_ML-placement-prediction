# End-to-End Machine Learning Project

## Overview

This project demonstrates a simple end-to-end machine learning workflow using Python and Scikit-learn. The model predicts student placement status based on two features:

* CGPA
* IQ

A Logistic Regression model is trained on the dataset and saved using Pickle for future deployment.

---

## Features

* Data loading using Pandas
* Basic data preprocessing
* Exploratory Data Analysis (EDA)
* Feature selection
* Train-test split
* Feature scaling using `StandardScaler`
* Logistic Regression model training
* Accuracy evaluation
* Decision boundary visualization
* Model saving using Pickle

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Mlxtend
* Pickle

---

## Project Workflow

### 1. Import Libraries

The project starts by importing required Python libraries.

### 2. Load Dataset

The dataset is loaded using Pandas:

```python
df = pd.read_csv('placement.csv')
```

### 3. Data Preprocessing

* Removes unnecessary columns
* Checks dataset information
* Visualizes data points

### 4. Feature Selection

Input features:

* CGPA
* IQ

Target feature:

* Placement

### 5. Train-Test Split

Dataset is divided into training and testing sets.

### 6. Feature Scaling

`StandardScaler` is used to normalize feature values.

### 7. Model Training

A Logistic Regression model is trained:

```python
clf = LogisticRegression()
clf.fit(X_train, Y_train)
```

### 8. Prediction & Evaluation

Predictions are made on test data and evaluated using accuracy score.

### 9. Decision Boundary Visualization

The decision regions are visualized using `mlxtend`.

### 10. Save Model

The trained model is saved as:

```python
model.pkl
```

---

## Installation

Install the required libraries before running the project:

```bash
pip install pandas numpy matplotlib scikit-learn mlxtend
```

---

## How to Run

1. Clone the repository
2. Install dependencies
3. Place the dataset file (`placement.csv`) in the project directory
4. Run the Python file:

```bash
python end_to_end__ml.py
```

---

## Output

The project generates:

* Trained Logistic Regression model
* Accuracy score
* Decision boundary visualization
* `model.pkl` saved model file

---

## Future Improvements

* Add more features for better prediction
* Use larger datasets
* Try advanced ML algorithms
* Deploy model using Flask or Streamlit
* Add hyperparameter tuning

---

## Author

Machine Learning Beginner Project for understanding the complete ML pipeline.
