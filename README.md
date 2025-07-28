# Nike Sales Exploratory Data Analysis (EDA)

### 📊 [View the Interactive Notebook on Kaggle](https://www.kaggle.com/code/kaustubhwaugh/nike-sales-eda-exploratory-data-analysis)

### Dataset - [Nike Sales Dataset](https://www.kaggle.com/datasets/nayakganesh007/nike-sales-uncleaned-dataset)

---

### 🎯 Project Objective
The goal of this analysis is to explore the Nike sales dataset to identify key drivers of revenue and profit. The project involves data cleaning, exploratory data analysis, and visualization to provide actionable insights for business improvement.

---

### 📈 Key Insights & Interpretation
This analysis uncovered several key findings:

* **Retail Dominance:** The Retail channel is the cornerstone of revenue and profitability, significantly outperforming the Online channel.
* **Geographic Concentration:** Sales are heavily concentrated in major metropolitan areas like Delhi and Mumbai, which are the leading regions in both total revenue and profit.
* **Top Product Lines:** Lifestyle and Running are the top two product lines by revenue. However, the Training product line shows a higher median profit margin, indicating strong per-item profitability.
* **Discounting Strategy Review:** The analysis revealed a clear negative correlation between the discount applied and the resulting profit margin. It also uncovered critical data anomalies, such as discounts exceeding 100%, which required correction.

---

### 🧹 Data Cleaning & Preprocessing
The initial dataset required significant cleaning and preprocessing to ensure the analysis was accurate:
* **Standardized Categorical Data:** Inconsistent region names (e.g., "Hyd", "hyderbad") were mapped to a standard format ("Hyderabad").
* **Handled Missing Values:** Missing `Discount_Applied` values were filled with 0, and rows with missing core financial data (`MRP`, `Units_Sold`) were dropped.
* **Corrected Financial Metrics:** The `Revenue` column was recalculated using the formula: `Revenue = MRP * Units_Sold * (1 - Discount_Applied)` to correct widespread zero-value entries.
* **Formatted Dates:** The `Order_Date` column, which contained multiple formats, was standardized to a datetime object for time-series analysis.

---

### 🛠️ Tech Stack & Libraries
* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

### 🚀 How to Run
1.  Clone this repository: `git clone https://github.com/kaustubhwaugh/Nike-Sales-Analysis.git`
2.  Install the required libraries: `pip install pandas numpy matplotlib seaborn`
3.  Open the `Nike_Sales.ipynb` file in Jupyter Notebook or JupyterLab.
