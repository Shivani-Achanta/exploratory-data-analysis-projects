# 📊 Banking Customer EDA Project

This project performs **Exploratory Data Analysis (EDA)** on a banking dataset sourced from a SQL Server database. The goal is to uncover trends, patterns, and insights that can support better decision-making for marketing, segmentation, and product offerings.

---

## 🔍 Project Overview

This EDA project investigates customer data from a banking database to:

- Understand demographic and financial profiles
- Identify patterns in credit, deposits, and account holdings
- Segment customers based on loyalty and fee structures
- Explore correlations and customer behavior

---

## 📊 Analysis Workflow

1. **Importing Libraries & Connecting to SQL**
2. **Data Extraction** from SQL Server using a custom SQL query
3. **Initial Data Exploration**
   - `df.head()`, `df.info()`, `df.describe()`
   - Missing value and duplicate checks
4. **Data Cleaning**
   - Convert `Joined_Bank` to datetime
   - Handle duplicates and formatting
5. **Univariate Analysis**
   - Value counts and distributions for categorical columns
   - Histograms for numerical features
6. **Bivariate Analysis**
   - Scatter plots, heatmaps, and grouped bar plots
7. **Feature Engineering**
   - Added `Tenure` feature from `Joined_Bank` column
8. **Visualization**
   - Count plots, histograms, heatmaps, and scatter plots using `seaborn` and `matplotlib`

---

## 📈 Key Insights

### 🧍‍♂️ Demographics & Segmentation
- **Nationality:** European segment dominates (1400+ customers).
- **Fee Structure:** High-fee customers form the largest group.
- **Loyalty Tier:** Majority in Jade tier, with room to grow Platinum.

### 💳 Financial Behavior
- **Credit Card Ownership:** Most customers have only 1 card.
- **Property Ownership:** Significant middle-class and high-net-worth segments.
- **Income Distribution:** Right-skewed with outliers; potential for high-end services.

### 🔄 Correlations
- **Deposits correlate strongly** with checking and savings accounts.
- **Credit card balance correlates with income**.

### ⏳ Tenure
- Recent surge in new customers (tenure ~5 years).
- Consistent long-term customer base between 15–30 years.

---

## 🚀 How to Run

1. Clone the repository:
   git clone https://github.com/your-username/banking-eda.git
   cd banking-eda

2. Install the dependencies:
   pip install -r requirements.txt

3. Run the notebook:
   - Open `banking_customer_eda.ipynb` in Jupyter or VSCode
   - Ensure your system has access to the SQL Server instance
