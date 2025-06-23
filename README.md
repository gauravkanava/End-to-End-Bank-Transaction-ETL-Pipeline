# End-to-End-Bank-Transaction-ETL-Pipeline

This project showcases a complete end-to-end ETL and data analysis pipeline built around real-world bank transaction data. It includes an ETL (Extract, Transform, Load) workflow, feature engineering, and exploratory visualizations—all using Python and popular data libraries.

---

## 📌 Project Highlights

- Cleaned messy transaction and date data
- Removed formatting characters like `$`, `,`, and placeholders like `#####`
- Converted date columns into proper `datetime` format
- Engineered new features like:
  - `transaction_hour`
  - `transaction_day`
  - `is_senior_citizen`
  - `amount_category`
- Visualized trends:
  - Daily transaction count
  - Customer age vs. transaction amount

---

## 🗂 Folder Structure

```
|-- End-to-End Bank Transacation ETL pipeline/
    |-- Bank_transactions_data.csv
    |-- Cleaned_bank_data.csv
    |-- main.ipynb
    |-- visualizations/
        |-- daily_transaction_counts.png
        |-- customer_age_vs_transaction_amount.png
    |-- README.md
```

---

## 🧠 Tech Stack

- **Python** - Core programming langauage
- **Pandas** - Data cleaning, ETL, and analysis
- **NumPy** - Numerical operations
- **Matplotlib & Seaborn** - Data visualization

---

## ⚙️ ETL Workflow

### Extract:
- Loaded raw bank transaction data from a CSV file.

### Transform:
- Standardized column names
- Replaced placeholder strings like `#####` with `NaN`
- Parsed date columns (`TransactionDate`, `PreviousTransactionDate`)
- Cleaned and converted monetary values (removed `$`, `,`)
- Engineered new features:
  - `transaction_hour`
  - `transaction_day`
  - `is_senior_citizen`
  - `amount_category` using `qcut`

### Load:
- Exported the cleaned data to `Cleaned_bank_data.csv` for further analysis and visualization.

---

## 📊 Visualizations

| Daily Transactions                         | Age vs. Transaction Amount            |
|-------------------------------------------|---------------------------------------|

---

## 💡 Key Insights

- **Daily transaction patterns** revealed fluctuations in banking activity, helping spot peak usage periods.
- **Customer age vs. transaction amount** showed useful behavioral patterns by age group.
- This project involved realistic data cleanup challenges (bad currency formatting, inconsistent dates, etc.) — making it ideal for showcasing ETL proficiency.

---
