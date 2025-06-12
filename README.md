# Telecom Customer Churn Analysis

This project analyzes customer behavior for a telecom company using real-world customer data. It focuses on answering specific business questions through data exploration, visualization, and statistical testing.

## Dataset Source

**Jafari-Marandi, R., Denton, J., Idris, A., Smith, B. K., & Keramati, A. (2020)**  
*Optimum Profit-Driven Churn Decision Making: Innovative Artificial Neural Networks in Telecom Industry*  
Published in *Neural Computing and Applications*

> Dataset includes 3,150 customer records with features such as call usage, complaints, subscription type, customer value, and churn status.

## Project Goals

This notebook is structured around three mini-challenges designed to explore different aspects of the dataset and demonstrate applied data science skills.

### Challenge 1: SMS vs Call Usage by Age Group
**Question:**  
Which age groups send more SMS messages than make phone calls?

**Skills:**  
- Grouped aggregation with `groupby()`
- Conditional logic and boolean masking
- Age-based behavior analysis

---

### Challenge 2: Visualizing Distinct Phone Calls by Call Length
**Question:**  
How does the number of distinct calls differ by age group and call length (Short, Medium, Long)?

**Skills:**  
- Feature engineering (binning with custom thresholds)
- Grouped aggregation and reshaping
- Visualization with `seaborn.barplot()`

---

### Challenge 3: Statistical Analysis by Tariff Plan
**Question:**  
Are there significant differences in call durations between pay-as-you-go and contractual customers?

**Skills:**  
- Hypothesis testing (Welch’s t-test)
- Statistical inference and interpretation
- Practical application of `scipy.stats.ttest_ind()`

---

## Technologies Used

- Python
- pandas, NumPy
- seaborn, matplotlib
- scipy

---

## Key Findings

- Age Groups **2** and **3** send more SMS than make calls.
- Long calls dominate across all age groups, especially in **Groups 2 and 3**.
- **Contractual customers (Plan 2)** make **significantly longer calls** than **pay-as-you-go users (Plan 1)**, with a p-value < 0.001.

---

## Skills Demonstrated

- Data wrangling and aggregation
- Exploratory Data Analysis (EDA)
- Statistical hypothesis testing
- Plotting and interpretation for business insights
- Communicating findings in a structured, interpretable format

---

## 📌 How to Run

1. Clone this repository  
2. Ensure `customer_churn.csv` is in a `data/` folder  
3. Run the notebook in Jupyter or VSCode

```bash
jupyter notebook telecom_churn_analysis.ipynb
