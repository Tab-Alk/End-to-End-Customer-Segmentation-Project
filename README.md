# Online Retail Customer Segmentation Analysis

## Introduction

This project undertakes a customer segmentation analysis using the Online Retail Dataset. The primary goal was to identify distinct groups of customers based on their purchasing behavior, employing RFM (Recency, Frequency, Monetary) metrics and K-Means clustering. The aim is to provide actionable insights that can help in tailoring marketing efforts and understanding customer value.

## Methodology

The approach to segmenting customers involved several key steps:

1.  **Data Preparation:** The initial phase involved loading the dataset, followed by essential cleaning processes. This included addressing records with missing `CustomerID`s, removing transactions corresponding to cancellations or returns, and ensuring data consistency for accurate analysis. A `TotalPrice` was also calculated for each relevant transaction.
2.  **RFM Feature Engineering:** For each unique customer, three key behavioral metrics were calculated:
    * Recency (R): Days since their last purchase.
    * Frequency (F): Total number of unique transactions.
    * Monetary Value (M): Total amount spent.
3.  **K-Means Clustering:** These RFM features were then standardized to ensure equal weighting, and the K-Means algorithm was applied to group customers into four distinct segments based on similarities in their RFM profiles.

## Customer Segments Visualization

The chart below illustrates the distinct profiles of the four customer segments identified through K-Means clustering, based on their average Recency, Frequency, and Monetary values.

<img width="1143" alt="Screenshot 2025-05-27 at 12 25 40 PM" src="https://github.com/user-attachments/assets/9674c93e-0152-436b-904e-26948478fabc" />

This visualization helps in understanding the defining characteristics of each segment at a glance. For instance, we can observe how segments differ in terms of recent purchasing activity, buying frequency, and overall spending.

## Key Insights from the Analysis

The segmentation analysis, particularly highlighted by the visualization above, revealed several key insights:

* **Four Distinct Segments:** The K-Means clustering effectively partitioned customers into four groups, each with a unique RFM signature.
* **Identification of a High-Value Segment:** One segment (Segment 2 in the notebook analysis) clearly stands out. As seen in the chart, these customers typically exhibit low recency (they've purchased recently), high frequency (they buy often), and high monetary value (they spend a lot).
* **Significant Revenue Contribution:** Further analysis showed that this high-value segment is responsible for approximately **18.58% of the total revenue**. This underscores their critical importance to the business.
* **Actionable Differences:** The other segments represent customers with different needs and behaviors—some might be newer customers with potential (e.g., moderate recency, lower frequency/monetary), while others might be at risk of churning (e.g., high recency, low frequency).

These findings allow for a more strategic approach to customer engagement, moving beyond generic campaigns to more personalized interactions.

## Conclusion & Key Learnings

This project successfully demonstrated how RFM analysis combined with K-Means clustering can be used to identify meaningful customer segments within a retail dataset. The process of transforming raw transactional data into these actionable insights was a key learning experience.

The most impactful takeaway is the quantification of a high-value customer segment and its significant contribution to revenue (18.58%). This highlights the practical value of segmentation in guiding business strategy, particularly in allocating marketing resources and developing targeted retention efforts. Understanding these distinct customer groups is the first step towards building stronger, more profitable customer relationships.
