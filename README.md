# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required libraries for data handling, plotting, and Decision Tree classification.

2.Load the Employee dataset and convert categorical data into numerical format using get_dummies().

3.Split the dataset into input features (X) and target output (y), then divide the data into training and testing sets.

4.Create and train the DecisionTreeClassifier model using the training data, then predict the output for test data.

5.Calculate the accuracy of the model and display the Decision Tree diagram using plot_tree().
## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeClassifier, plot_tree
from sklearn.metrics import accuracy_score
data = pd.read_csv("Employee.csv")
data = pd.get_dummies(data, drop_first=True)
X = data.iloc[:, :-1]
y = data.iloc[:, -1]
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)
model = DecisionTreeClassifier(random_state=42)
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
print("Accuracy:", accuracy_score(y_test, y_pred))
plt.figure(figsize=(20,10))

plot_tree(
    model,
    feature_names=X.columns,
    filled=True
)

plt.show()

Developed by: R.Rachanaa
RegisterNumber: 212225040322 
*/
```

## Output:
Accuracy: 0.896

<img width="1237" height="612" alt="image" src="https://github.com/user-attachments/assets/cc9ee6da-5f47-4e01-93e4-6cd7b0603f9f" />


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
