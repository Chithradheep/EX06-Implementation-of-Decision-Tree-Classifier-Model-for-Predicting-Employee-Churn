# EX 6 Implementation of Decision Tree Classifier Model for Predicting Employee Churn
## DATE:
## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Clean data, handle missing values, encode categorical features, and split into training/testing sets.
2. Initialize DecisionTreeClassifier() and fit it using the training data.
3. Use the trained model to predict employee churn on the test set.
4. Measure accuracy and other metrics like precision, recall, and F1-score to assess model performance.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Chithradheep R
RegisterNumber:  2305002003

import pandas as pd
from sklearn.tree import DecisionTreeClassifier , plot_tree
from sklearn.preprocessing import LabelEncoder
import matplotlib.pyplot as plt
df=pd.read_csv("/content/Employee_EX6.csv")
data=df.copy()
data
le=LabelEncoder()
data['salary']=le.fit_transform(data['salary'])
data
x=data.drop(['Departments','left'],axis=1)
y=data['left']
clf=DecisionTreeClassifier()
clf.fit(x,y)
plt.figure(figsize=(80,80))
plot_tree(clf,filled=True,feature_names=x.columns,class_names=['LEFT','NOT LEFT'])
plt.show()

*/
```

## Output:

![Screenshot 2024-10-10 143608](https://github.com/user-attachments/assets/4d63dac0-2052-4dde-aeac-ec333a063fa6)
![Screenshot 2024-10-10 143649](https://github.com/user-attachments/assets/7635eca3-9996-47d5-8baf-66cb118c6c22)
![Screenshot 2024-10-10 143733](https://github.com/user-attachments/assets/5a5d76c1-4cd0-471a-97c7-12147ef5acdc)
![Screenshot 2024-10-10 143920](https://github.com/user-attachments/assets/5db50e31-3bc6-4722-b9f6-b0d08358e417)
![Screenshot 2024-10-10 143951](https://github.com/user-attachments/assets/7615a477-c95a-4cd5-9d7a-5c6e5593a0eb)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
