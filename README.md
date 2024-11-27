# Customer Segmentation Project using RFM and K-Means Clustering

## Table of Contents
- [Introduction](#introduction)
- [Importance of Customer Segmentation](#importance-of-customer-segmentation)
- [Objectives](#objectives)
- [RFM Analysis](#rfm-analysis)
- [K-Means Clustering](#k-means-clustering)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Conclusion](#conclusion)
- [How to Run the Project](#how-to-run-the-project)

---

## Introduction
This project focuses on customer segmentation using the RFM (Recency, Frequency, and Monetary) model combined with **K-Means clustering**. Customer segmentation is the process of dividing a company's customer base into groups that are similar in specific ways relevant to marketing, such as age, gender, interests, or spending habits.

Customer segmentation is essential for understanding customer behavior, improving customer satisfaction, increasing engagement, and optimizing marketing campaigns.

---

## Importance of Customer Segmentation
Customer segmentation enables businesses to:
- **Identify customer needs**: Segmenting customers helps businesses identify and cater to specific customer needs.
- **Improve marketing strategies**: Businesses can craft tailored marketing messages that resonate with different customer groups.
- **Increase customer retention**: By understanding customer behavior through segmentation, businesses can engage more effectively, improving loyalty and reducing churn.
- **Boost profitability**: Focused marketing efforts and personalized experiences often result in increased sales and customer lifetime value.

---

## Objectives
The main objectives of this project are:
1. **Segment customers** based on their purchasing behavior using RFM analysis.
2. **Apply K-Means clustering** to group customers into distinct segments.
3. Provide insights into each customer segment for **targeted marketing** strategies.
4. Visualize the clusters to understand customer distribution.

---

## RFM Analysis
The **RFM** model stands for:
- **Recency**: How recently a customer has made a purchase.
- **Frequency**: How often a customer makes a purchase.
- **Monetary Value**: How much money a customer has spent on purchases.

### Why RFM?
RFM analysis is used to analyze customer value and identify customers who are more likely to respond to promotions or loyalty programs. It is simple, yet effective, because it directly relates to customer behavior in ways that are easy to interpret.

---

## K-Means Clustering
K-Means is an unsupervised machine learning algorithm that is used for clustering data into different groups or clusters. It aims to partition customers into **K distinct clusters** based on their RFM values, ensuring that customers within the same cluster are more similar to each other than to those in other clusters.

### Why K-Means?
- K-Means is an easy-to-implement, efficient algorithm for large datasets.
- It helps visualize customer segments effectively by assigning customers to clusters based on their behavior patterns.

---

## Dataset
The dataset used for this project contains customer purchase data that includes:
- **Customer ID**: Unique identifier for each customer.
- **Invoice No**: Transaction details.
- **Purchase Date**: Date of the purchase.
- **Amount Spent**: The total monetary value of the purchase.

The dataset is used to calculate RFM scores for each customer, which serve as the input for clustering.

---

## Methodology
The process for performing customer segmentation is as follows:

1. **Data Preprocessing**:
   - Data cleaning (handling missing values, duplicates).
   - Feature extraction for Recency, Frequency, and Monetary (RFM) metrics.

2. **RFM Analysis**:
   - Calculate RFM scores for each customer.
   - Standardize the RFM values to avoid biases in clustering.

3. **K-Means Clustering**:
   - Apply the Elbow Method to determine the optimal number of clusters.
   - Implement K-Means clustering on the RFM scores to group customers.

4. **Visualization**:
   - Use PCA (Principal Component Analysis) for dimensionality reduction.
   - Plot clusters to visualize customer segmentation.

---

## Results
The clustering analysis generated the following customer segments:

### Cluster 0: Infrequent, Low-Value Customers
- **Recency**: Moderate
- **Frequency**: Low
- **Monetary**: Low
- **Description**: These customers haven't made a purchase recently and don't buy frequently or spend much. This group likely represents infrequent, low-value customers or those who may be at risk of churning.

### Cluster 1: Churning Customers
- **Recency**: High
- **Frequency**: Low
- **Monetary**: Low
- **Description**: This cluster includes customers who made a purchase a long time ago, don't buy often, and don't spend much. They may represent churning customers who are disengaged and potentially need re-engagement strategies.

### Cluster 2: Most Loyal, High-Value Customers
- **Recency**: Low
- **Frequency**: Very High
- **Monetary**: Very High
- **Description**: These customers have purchased recently, buy very frequently, and spend a lot. This group likely represents your most loyal, high-value customers who frequently engage and spend significantly.

### Cluster 3: Active, Valuable Customers
- **Recency**: Low
- **Frequency**: Moderate
- **Monetary**: Moderate
- **Description**: These customers made a purchase recently, buy somewhat frequently, and spend a decent amount. This group likely represents active, valuable customers, though not as high-value as those in Cluster 2.


The **Elbow Method** was used to identify that **3 or 4 clusters** are optimal, balancing simplicity and detail.

---

## Conclusion
The customer segmentation based on the RFM model and K-Means clustering helps businesses better understand their customer base. By identifying these four distinct customer segments, businesses can apply tailored strategies to enhance customer retention, optimize marketing efforts, and ultimately increase profitability. The next steps could include deploying targeted marketing campaigns for each segment, developing loyalty programs for high-value customers, and re-engagement efforts for those at risk of churn.
 key customer groups, companies can target their marketing efforts more effectively, boost customer retention, and increase overall profitability.

---

## How to Run the Project
To run this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/compbio-chuma/Customer_segmentation_rfm.git
   cd Customer_Segmentation_rfm
