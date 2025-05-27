# Customer Segmentation Analysis for Online Retail

## Project Overview

This project performs a customer segmentation analysis on the Online Retail Dataset to identify distinct customer groups based on their purchasing behavior. By applying RFM (Recency, Frequency, Monetary) analysis and K-Means clustering, the goal is to uncover actionable insights that can inform targeted marketing strategies and enhance customer engagement. The core aim is to understand different customer archetypes and quantify the value of key segments.

## Methodology

The analytical process comprised several key stages:

1.  **Data Preparation:** The Online Retail dataset (UCI Machine Learning Repository) was loaded and cleaned. This involved handling missing `CustomerID` values, removing cancelled or invalid transactions, and calculating `TotalPrice` for each transaction.
2.  **RFM Feature Engineering:** For each unique customer, Recency (days since last purchase), Frequency (total number of transactions), and Monetary value (total amount spent) were computed.
3.  **Customer Segmentation:** The RFM features were standardized, and K-Means clustering (using 4 clusters) was applied to group customers into distinct segments based on their RFM profiles.

## Key Findings & Insights

The segmentation revealed four distinct customer groups. A significant finding is the identification of a **high-value segment (Segment 2 in the notebook analysis)**.

* This key segment, distinguished by recent purchases, high purchase frequency, and substantial monetary spending, accounts for approximately **18.58% of the total revenue**.
* This concentration of revenue highlights the strategic importance of this group and enables the development of targeted retention and engagement strategies. Other segments represent customers with different patterns, such as newer or at-risk individuals, also offering opportunities for tailored approaches.

These insights provide a data-driven basis for optimizing marketing efforts and improving customer relationship management.

## Core Libraries Utilized

The analysis primarily leveraged the following Python libraries:
* **Pandas:** For data manipulation and RFM calculations.
* **Scikit-learn:** For feature scaling and K-Means clustering.
* **Matplotlib & Seaborn:** For visualizing segment profiles and distributions.

## Visualizing the Segments (Recommended)

Including a visualization in your README can greatly enhance its impact by providing an immediate visual summary of your findings.

**Why include one?**
* A chart can quickly convey the differences between segments (e.g., average RFM values).
* It makes your project more engaging and easier to understand at a glance.

**What to include?**
A good candidate would be the **Segment Profile Bar Chart** you generated, showing the average Recency, Frequency, and Monetary value for each of the 4 segments.

**How to add it to your GitHub README:**
1.  **Save your plot:** From your Jupyter Notebook, save the chosen visualization as an image file (e.g., `segment_profiles.png`) in your project directory. It's good practice to create an `assets` or `images` subfolder for this (e.g., `assets/segment_profiles.png`).
2.  **Commit the image:** Add and commit this image file to your GitHub repository.
3.  **Embed in README:** Use the following Markdown syntax in your README file:
    ```markdown
    ![Segment Profiles](assets/segment_profiles.png)
    ```
    *(Adjust the path `assets/segment_profiles.png` if you place the image elsewhere.)*

## Conclusion

This project successfully segmented customers from the Online Retail dataset, identifying key groups and quantifying the significant impact of high-value customers. These insights are valuable for developing more focused and effective business strategies.

## Potential Enhancements

* Systematic determination of the optimal number of clusters.
* Tracking customer segment changes over time.
* Incorporating additional data features for richer segmentation.
