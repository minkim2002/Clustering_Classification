# 🌸 Iris Classification using KNN and K-Means

# 📊 KNN and K-means Classification

![Python](https://img.shields.io/badge/python-3.x-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/pandas-1.x-orange?style=for-the-badge&logo=pandas)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-0.24-green?style=for-the-badge&logo=scikit-learn)
![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)

This repository contains Python implementations of **K-Nearest Neighbors (KNN)** and **K-means clustering** algorithms to classify and cluster the Iris dataset.  
Both **KNN** and **K-means** models support training, prediction, and visualization using the Iris dataset.

---

## 🚀 Features

### KNN (K-Nearest Neighbors):
✅ Train a KNN model to classify Iris flowers based on sepal and petal measurements  
✅ Predict the label of the test dataset using the trained model  
✅ Supports dynamic selection of the number of neighbors (k)  
✅ Easy to modify distance metric (Euclidean in this case)  

### K-means:
✅ Implement the K-means clustering algorithm  
✅ Classify data points into k clusters based on similarity  
✅ Recalculate centroids iteratively until convergence  
✅ Test the trained K-means model on a validation set  

---

## ⚙️ Requirements

- Python 3.x  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- seaborn  

Install all dependencies:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn

## 🧑‍💻 How to Run

### **Run KNN Algorithm**

To train and test the KNN model, use the following command:

python knn.py -mode train -k 3 -num_epochs 25
python knn.py -mode test

python kmeans.py -mode train -k 3 -num_epochs 25
python kmeans.py -mode test
