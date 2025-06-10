
# 🛒 E-commerce Return Rate Reduction Analysis

This project aims to identify and reduce product return rates in an e-commerce environment using data cleaning, exploratory analysis, return rate metrics, machine learning prediction, and interactive dashboarding.

---

## 📁 Repository Structure

```
├── raw_data.zip                  # Original raw datasets
├── cleaned_data.zip              # Cleaned and processed datasets
├── Data Cleaning.ipynb           # Step 1: Data preprocessing & cleaning
├── Return Percentage.ipynb       # Step 2: Return rate analysis
├── Prediction.ipynb              # Step 3: Logistic regression modeling
├── Ecommerce Analysis.pbix       # Step 4: Interactive dashboard in Power BI
└── README.md
```

---

## 🔁 Project Workflow

### ✅ Step 1: Data Cleaning [`Data Cleaning.ipynb`]
- Loaded 9 raw datasets covering orders, customers, products, refunds, ratings, subscriptions, etc.
- Performed standardization: column names and values converted to lowercase.
- Merged and formatted date/time fields.
- Handled missing values and inconsistent entries.
- Exported cleaned datasets into a separate ZIP file for easy reuse.

### 📊 Step 2: Return Rate Analysis [`Return Percentage.ipynb`]
- Merged orders with return and refund records.
- Calculated return percentages across:
  - Product categories
  - Suppliers
  - State
- Identified high-return categories to focus intervention strategies.

### 🤖 Step 3: Return Prediction Model [`Prediction.ipynb`]
- Used cleaned datasets to build a logistic regression model.
- Target: Probability of a product being returned.
- Performed:
  - Feature engineering (e.g., encoding, normalization)
  - Model training, validation, and ROC-AUC evaluation.
- Exported high-risk products list based on model probabilities.

### 📈 Step 4: Power BI Dashboard [`Ecommerce Analysis.pbix`]
- Visualized key metrics:
  - Return rates over category, Suppliers and State
  - Total vs Returned Orders by Category and States
  - Matrix of Retuen yate Percentage and Return Propability
- Enabled dynamic filtering and drill-downs for data storytelling.
![image](https://github.com/user-attachments/assets/83a17222-6e22-45ce-879e-e7b82b22af81)
![image](https://github.com/user-attachments/assets/77283939-82b6-4168-b034-bebe889282dc)



---

## 📦 Datasets

Two ZIPs are included for reproducibility:

- `raw_data.zip`: Original, unprocessed datasets.
- `cleaned_data.zip`: Final cleaned versions used in analysis and modeling.

---

## 🧠 Goal

To help e-commerce businesses proactively minimize return rates by:
- Identifying return patterns
- Predicting return probability before delivery
- Informing supply chain and customer policy decisions

---

## 🛠️ Tech Stack

- Python (Pandas, Scikit-learn, Matplotlib, Seaborn)
- Power BI for data storytelling
- Jupyter Notebooks
- Logistic Regression Model
- CSV/ZIP file handling

---

## 📌 How to Use

1. Unzip and review `raw_data.zip` or start directly with `cleaned_data.zip`.
2. Open notebooks in the following order:
   - `Data Cleaning.ipynb`
   - `Return Percentage.ipynb`
   - `Prediction.ipynb`
3. Explore interactive visuals in `Ecommerce Analysis.pbix` via Power BI Desktop.
