# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
1.Import the libraries and read the data frame using pandas.
2.Calculate the null values present in the dataset and apply label encoder.
3.Determine test and training data set and apply decison tree regression in dataset.
4.Calculate Mean square error,data prediction and r2.

## Program:
```
/*
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: magesh v
RegisterNumber:212222040092
import pandas as pd
import matplotlib.pyplot as plt
data=pd.read_csv('/content/Mall_Customers.csv')

data.head()

data.info()

data.isnull().sum()

from sklearn.cluster import KMeans
wcss=[]

for i in range (1,11):
  kmeans=KMeans(n_clusters=i,init="k-means++")
  kmeans.fit(data.iloc[:,3:])
  wcss.append(kmeans.inertia_)
km=KMeans(n_clusters = 5)
km.fit(data.iloc[:,3:])

y_pred=km.predict(data.iloc[:,3:])
y_pred

data["cluster"]=y_pred
df0 = data[data["cluster"]==0]
df1 = data[data["cluster"]==1]
df2 = data[data["cluster"]==2]
df3 = data[data["cluster"]==3]
df4 = data[data["cluster"]==4]
plt.scatter(df0["Annual Income (k$)"],df0["Spending Score (1-100)"],c="mediumpurple",label="cluster0")
plt.scatter(df1["Annual Income (k$)"],df1["Spending Score (1-100)"],c="darkseagreen",label="cluster1")
plt.scatter(df2["Annual Income (k$)"],df2["Spending Score (1-100)"],c="lightskyblue",label="cluster2")
plt.scatter(df3["Annual Income (k$)"],df3["Spending Score (1-100)"],c="green",label="cluster3")
plt.scatter(df4["Annual Income (k$)"],df4["Spending Score (1-100)"],c="pink",label="cluster4")
plt.legend()
plt.title("Customer Segments")

*/  
*/
```

## Output:
data.head()
![image](https://github.com/magesh534/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135577936/0b1bfc4f-1060-43af-a4ae-28e95387c14d)

data.info()
![image](https://github.com/magesh534/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135577936/370b95ae-57d2-4580-8f74-4ec6b178de19)

isnull() and sum()
![image](https://github.com/magesh534/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135577936/e797a003-93f2-4b10-b6c8-45b03d75af9b)

data.head() for salary
![image](https://github.com/magesh534/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135577936/8b0f4cbb-e8a9-49e4-9050-0fd552aa9ac8)

MSE value
![image](https://github.com/magesh534/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135577936/1ee1f5f4-7611-4aeb-a404-5dabd139dbf1)

r2 value
![image](https://github.com/magesh534/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135577936/69e9a7ed-194e-4d4b-9765-636ff410afe8)

data prediction
![image](https://github.com/magesh534/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135577936/68ea8e04-8ef7-4876-9a21-2854e1898637)

## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
