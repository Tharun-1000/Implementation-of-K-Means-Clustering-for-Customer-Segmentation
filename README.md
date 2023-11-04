![image](https://github.com/Tharun-1000/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135952958/eee21a7a-08c6-420a-bb64-c56992bc78e5)# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the necessary packages using import statement.
2.Read the given csv file using read_csv() method and print the number of contents to be displayed
using df.head().
3.Import KMeans and use for loop to cluster the data.
4.Predict the cluster and plot data graphs.
5.Print the outputs and end the program

## Program:

/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: THARUN K
RegisterNumber:  212222040172

import pandas as pd
import matplotlib.pyplot as plt
data = pd.read_csv("/content/Mall_Customers (1).csv")
data.head()
data.isnull().sum()
from sklearn.cluster import KMeans
wcss=[]
for i in range(1,11):
kmeans=KMeans(n_clusters=i,init="k-means++")
kmeans.fit(data.iloc[:,3:])
wcss.append(kmeans.inertia_)
plt.plot(range(1,11),wcss)
plt.xlabel("No.of clusters")
plt.ylabel("wcss")
plt.title("Elbow Method")
km=KMeans(n_clusters=5)
km.fit(data.iloc[:,3:])
y_pred=km.predict(data.iloc[:,3:])
y_pred
data["cluster"]=y_pred
df0=data[data["cluster"]==0]
df1=data[data["cluster"]==1]
df2=data[data["cluster"]==2]
df3=data[data["cluster"]==3]
df4=data[data["cluster"]==4]
plt.scatter(df0["Annual Income (k$)"],df0["Spending Score (1-100)"],c="red",label="clu
plt.scatter(df1["Annual Income (k$)"],df1["Spending Score (1-100)"],c="black",label="c
plt.scatter(df2["Annual Income (k$)"],df2["Spending Score (1-100)"],c="blue",label="cl
plt.scatter(df3["Annual Income (k$)"],df3["Spending Score (1-100)"],c="green",label="c
plt.scatter(df4["Annual Income (k$)"],df4["Spending Score (1-100)"],c="magenta",label=
plt.legend()
plt.title("Customer Segments")

*/


## Output:

data.head()

![image](https://github.com/Tharun-1000/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135952958/bcfddbb5-f507-4412-a320-a839ce453188)

DATA.info():

![image](https://github.com/Tharun-1000/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135952958/d9277a24-7985-46ce-a8c3-94831079b15e)

NULL VALUES

![image](https://github.com/Tharun-1000/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135952958/5f66ef97-5e95-4c01-9bdc-4df45c9be0c5)

ELBOW GRAPH:

![image](https://github.com/Tharun-1000/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135952958/df4b72c1-3137-46cd-9b2b-27c0d1f0bab4)

CLUSTER FORMATION:

![image](https://github.com/Tharun-1000/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135952958/60b87caf-fc25-4b31-9130-030e47e01605)

PREDICICTED VALUE:

![image](https://github.com/Tharun-1000/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135952958/88f01840-e5f2-4de5-855b-4b466a2ee50a)

FINAL GRAPH(D/O):

![image](https://github.com/Tharun-1000/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/135952958/5df38342-b124-4908-86b5-1145468004a7)





## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
