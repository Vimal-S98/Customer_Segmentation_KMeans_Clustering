# Customer Segmentation Using Clustering

## Project Overview
This project analyzes mall customer data to understand patterns in **Age**, **Annual Income**, and **Spending Score**. We perform **Exploratory Data Analysis (EDA)** and **K-Means clustering** to segment customers.

## Dataset
The dataset `Mall_Customers.csv` contains:

- `CustomerID` – Unique ID  
- `Gender` – Male/Female  
- `Age` – Age of the customer  
- `Annual Income (k$)` – Annual income in thousand dollars  
- `Spending Score (1-100)` – Customer spending score  

## Libraries Used
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikitlearn - KMeans

## Exploratory Data Analysis (EDA)
### Dataset Info
- Shape: (number_of_rows, number_of_columns)
- Missing values: none

## Key Charts

1. Distribution of Numerical Columns
<img width="1135" height="286" alt="image" src="https://github.com/user-attachments/assets/45ef3f19-6a6d-4c79-b74a-a5674029aac9" />

2. Income vs Spending Score (Scatterplot)
<img width="583" height="428" alt="image" src="https://github.com/user-attachments/assets/53e0dd86-c8e8-4329-8232-598a557cbefb" />

3. Correlation Heatmap
<img width="570" height="467" alt="image" src="https://github.com/user-attachments/assets/5b8cdb7c-1604-492f-9963-0168b3d1339d" />


## Clustering
### 1. Univariate Clustering (Annual Income)
- Elbow method suggested K=3
- Clustered customers based on Annual Income:
<img width="538" height="382" alt="image" src="https://github.com/user-attachments/assets/dc40eae6-b952-419d-8da4-926fdc5e8569" />
<br>
<img width="377" height="72" alt="image" src="https://github.com/user-attachments/assets/e244e554-9f30-41f7-8878-e7d15c9be395" />

### 2. Bivariate Clustering (Income & Spending)
- Elbow method suggested K=6
<img width="552" height="393" alt="image" src="https://github.com/user-attachments/assets/35ebdf28-020b-40df-abf3-fdbc905d0287" />


### Centroids
<img width="726" height="562" alt="image" src="https://github.com/user-attachments/assets/949599e4-81a7-4b91-b102-b2b80f8ee7c6" />

### 3. Multivariate Clustering
- Used Age, Annual Income, Spending Score, and one-hot encoded Gender
- Standardized features before clustering
- Final clustering with K=7
<img width="550" height="118" alt="image" src="https://github.com/user-attachments/assets/1788553f-e3e3-4778-a38c-43b99d11b23e" />
<img width="543" height="377" alt="image" src="https://github.com/user-attachments/assets/f2924f00-258a-4dbd-b3f9-1df627436c57" />

## Key Insights
- Customers can be segmented by income and spending habits
- Some clusters show high income & low spending, others low income & high spending
- Gender distribution varies slightly across clusters




