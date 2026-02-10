Customer Segmentation using RFM Analysis & K-Means Clustering
📌 Project Overview

This project focuses on segmenting customers based on their purchasing behavior using RFM analysis (Recency, Frequency, Monetary) and K-Means clustering.
The goal is to identify meaningful customer groups to support targeted marketing, retention strategies, and business decision-making.

📂 Dataset

The dataset consists of retail transaction data containing:

CustomerID

InvoiceDate

InvoiceNo

Quantity

UnitPrice

Each row represents a customer transaction.

🛠 Methodology

1. Data Cleaning & Preprocessing

Converted InvoiceDate to datetime format

Removed invalid transactions (negative quantity and monetary values)

Created TotalAmount = Quantity × UnitPrice

2. RFM Feature Engineering

Recency: Days since the last purchase using a snapshot date

Frequency: Number of unique invoices per customer

Monetary: Total spending per customer

3. Exploratory Data Analysis (EDA)

Analyzed RFM distributions

Identified and treated outliers to reduce skewness

4. Feature Scaling

Applied StandardScaler to normalize RFM values

5. K-Means Clustering

Used the Elbow Method and Silhouette Score to select the optimal number of clusters

Assigned cluster labels to customers

6. Visualization & Insights

Visualized customer distribution across clusters

Used 2D and 3D scatter plots to interpret customer behavior

📈 Key Insights

Identified high-value and loyal customers

Detected at-risk customers requiring re-engagement

Recognized low-value customer segments

🧰 Tools & Technologies

Python

Pandas, NumPy

Matplotlib, Seaborn, Plotly

Scikit-learn

✅ Conclusion

This project demonstrates how RFM analysis combined with K-Means clustering can effectively segment customers and generate actionable business insights.
