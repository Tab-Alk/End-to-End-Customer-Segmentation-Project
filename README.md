# End-to-End-Customer-Segmentation-Project

This project focuses on customer segmentation using the Online Retail Dataset. Python, along with libraries such as Pandas, Scikit-learn, Matplotlib, and Seaborn, was employed to perform RFM (Recency, Frequency, Monetary) analysis and K-Means clustering. The objective was to identify distinct customer groups based on their purchasing behavior and to quantify the significance of high-value segments.

## Key Findings

The analysis successfully grouped customers into four distinct segments. A significant outcome was the identification of a high-value customer segment (referred to as Segment 2 in the accompanying notebook).

* This high-value segment, characterized by high frequency and monetary values, and low recency, contributes approximately **18.58% of the total revenue**.
* Other identified segments generally represent customer groups such as potential loyalists, at-risk customers, and consistent spenders, each with distinct RFM characteristics.

Understanding these segments allows for more targeted marketing strategies and resource allocation.

## Getting Started

To run this project locally, please follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YourUsername/YourRepositoryName.git](https://github.com/YourUsername/YourRepositoryName.git)
    cd YourRepositoryName
    ```
    *(Replace `YourUsername/YourRepositoryName` with your specific GitHub path.)*

2.  **Dataset:**
    * The project utilizes the "Online Retail Dataset" from the UCI Machine Learning Repository.
    * Ensure the `OnlineRetail.csv` file is placed within a `data/raw/` directory in the project's root folder (i.e., `data/raw/OnlineRetail.csv`).

3.  **Install Dependencies:**
    The project requires the following Python libraries. These can be installed using pip:
    ```bash
    pip install pandas scikit-learn matplotlib seaborn jupyter
    ```

4.  **Execute the Notebook:**
    The primary analysis is contained within the Jupyter Notebook (`CustomerSegmentation.ipynb` or your specified filename). Open and run the notebook:
    ```bash
    jupyter notebook CustomerSegmentation.ipynb
    ```

## Technologies Used

* **Python 3.x**
* **Pandas:** Utilized for data manipulation, cleaning, and RFM feature calculation.
* **Scikit-learn:** Employed for data scaling (`StandardScaler`) and K-Means clustering (`KMeans`).
* **Matplotlib & Seaborn:** Used for generating visualizations of customer segments and their profiles.
* **Jupyter Notebook:** Served as the environment for code development, analysis, and documentation.

## Dataset Reference

* **Name:** Online Retail Dataset
* **Source:** UCI Machine Learning Repository.
    (Acknowledgements: Dr. Daqing Chen, Director of Public Analytics group at London South Bank University).
* **Relevant Columns:** `InvoiceNo`, `InvoiceDate`, `CustomerID`, `Quantity`, `UnitPrice`.

## Potential Enhancements

* Longitudinal analysis of segment migration over time.
* Exploration of alternative clustering algorithms or feature engineering techniques.
* Development of predictive models for new customer segmentation.

---

This README provides a concise and professional overview of the project.
