# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Start the program
2. Import the python pandas library as pd
3. Read the contents of the Spam csv file
4. Display the first 5 rows of the dataset using head()
5. Assign x as v1 values and y as v2 values
6. From sklearn library select the feature extraction and import CountVectorizer
7. CountVectorizer will convert the Text to Numerical Data
8. From sklearn library import Support Vector Classifier (ie. SVC)
9. Predict the x_test using SVC
10. Print the accuracy of the SVM Model 11.Stop the program
## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: VESLIN ANISH A
RegisterNumber: 212223240175
*/
```
```
/*
import chardet
file='/content/spam.csv'
with open(file, 'rb') as rawdata:
  result = chardet.detect(rawdata.read(100000))
result

import pandas as pd
data=pd.read_csv("/content/spam.csv",encoding = 'Windows-1252')

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values

y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv = CountVectorizer()

x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```
## Output:

 Result Output:

![image](https://github.com/user-attachments/assets/9977fa47-6a15-4679-9f92-8b9085fe0e86)


Data.head():

![image](https://github.com/user-attachments/assets/53c45b1e-038e-4250-a192-5664bc72221d)


Data.info():

![image](https://github.com/user-attachments/assets/48f86c56-1bcf-4876-86af-bb4a29681d2e)


Data.insull().sum():

![image](https://github.com/user-attachments/assets/0cf83fb6-6e89-4106-b354-3a986adef9e8)

Y_Prediction Value:

![image](https://github.com/user-attachments/assets/9aad1b17-15d6-4c4e-a265-ae795eb8b5c1)

Accuracy Value:

![image](https://github.com/user-attachments/assets/e31541b4-a4ba-4764-84b2-42cecd03eb64)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
