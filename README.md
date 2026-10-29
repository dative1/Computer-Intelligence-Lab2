# Computer Intelligence Lab 2
**Reg No: 224005548**

## Overview
This repository contains my submission for Lab 2. The goal of this assignment is to apply unsupervised machine learning techniques to the Country Schools Dataset to perform anomaly detection and cluster analysis.

## 1. Data Preprocessing
Before running the algorithms, the dataset was cleaned and prepared:
- Dropped empty rows and the overall "TOTAL" summary row.
- Corrected the county name "ElGEYO" to "ELGEYO MARAKWET".
- Converted `PercentageInstalled` from a string format (e.g., '10.34%') to numeric floats.
- Dropped irrelevant identifier columns (`SNO` and `FID`).
- Standardized all numerical features using `StandardScaler` for better algorithm performance.

## 2. Anomaly Detection
I applied the **Isolation Forest** algorithm to identify counties with unusual school installation metrics.
- **Normal counties:** 42
- **Anomalous counties:** 5
- **Detected Anomalies:** Turkana, Kitui, Makueni, Kakamega, and Machakos.

## 3. Cluster Analysis
I used **K-Means Clustering** to group similar counties. I evaluated cluster sizes from 2 to 10 using the Elbow Method and Silhouette Scores.
- **Selected clusters:** 8
- **Silhouette Score:** ~0.428

## 4. Visualization
The notebook includes visual outputs for:
- Anomaly Detection Scatter Plot
- Elbow Method Curve
- K-Means Cluster Groupings

## Tools Used
- Python
- Pandas & NumPy
- Scikit-learn
- Matplotlib
- Kaggle Notebook

## Notebook File
The `.ipynb` file in this repository contains all the Python code, data analysis, and visual plots.
