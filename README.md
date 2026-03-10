# BLENDED_LEARNING
# Implementation of Decision Tree Model for Tumor Classification

## AIM:
To implement and evaluate a Decision Tree model to classify tumors as benign or malignant using a dataset of lab test results.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
Load Data
1. Import the dataset to initiate the analysis.

Explore Data
2. Examine the dataset to identify patterns, distributions, and relationships.

Select Features
3. Determine the most important features to enhance model accuracy and efficiency.

Split Data
4. Separate the dataset into training and testing sets for effective validation.

Train Model
5. Use the training data to build and train the model.

Evaluate Model
6. Measure the model’s performance on the test data with relevant metrics.

## Program:
```
/*
Program to  implement a Decision Tree model for tumor classification.
Developed by: DEVENDRAN G
RegisterNumber:  212225240030

# Import necessary libraries
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeClassifier
from sklearn.metrics import accuracy_score, classification_report, confusion_matrix
import seaborn as sns
import matplotlib.pyplot as plt

# Step 2: Data Exploration
# Display the first few rows and column names for verification
print(data.head())
print(data.columns)

X = data.drop(columns=['Class'])  
y = data['Class']  


X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)


model = DecisionTreeClassifier(random_state=42)
model.fit(X_train, y_train)

y_pred = model.predict(X_test)

accuracy = accuracy_score(y_test, y_pred)
print("Accuracy:", accuracy)
print("Classification Report:\n", classification_report(y_test, y_pred))


conf_matrix = confusion_matrix(y_test, y_pred)
sns.heatmap(conf_matrix, annot=True, fmt="d", cmap="Blues")
plt.xlabel("Predicted")
plt.ylabel("Actual")
plt.title("Confusion Matrix")
plt.show()
*/
```

## Output:
![alt text](<Screenshot 2026-03-10 141509.png>)
![alt text](<Screenshot 2026-03-10 141532.png>)
![alt text](<Screenshot 2026-03-10 141543.png>)
## Result:
Thus, the Decision Tree model was successfully implemented to classify tumors as benign or malignant, and the model’s performance was evaluated.
