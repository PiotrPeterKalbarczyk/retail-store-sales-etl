# 📊 Retail Store Sales - ETL Pipeline

## 📝 Project: ETL for Retail Sales Data
This project demonstrates a simple **ETL (Extract, Transform, Load)** process for retail sales data. The data is extracted from a CSV file, cleaned and transformed using Python, and then loaded into a PostgreSQL database.

---

## 🔹 1. EXTRACT (Data Extraction)
✅ Load data from `retail_store_sales.csv` into a Pandas DataFrame.
✅ Perform basic data analysis (`head()`, `info()`, `describe()`).

---

## 🔹 2. TRANSFORM (Data Cleaning and Preparation)
✅ Remove duplicates.
✅ Standardize column names (lowercase, replace spaces with `_`).
✅ Convert `transaction_date` to `datetime` format.
✅ Handle missing values:
   - Fill `price_per_unit` using the first available value for each `item`.
   - Calculate `total_spent` as `price_per_unit * quantity`.
   - Fill missing values in `discount_applied` with `No`.
✅ Remove rows where `item` is `NaN`.

---

## 🔹 3. LOAD (Loading Data into PostgreSQL)
✅ Connect to PostgreSQL using `SQLAlchemy`.
✅ Create a table if it does not exist.
✅ Load data into PostgreSQL using `to_sql()`.

📌 **Note:** Database credentials (username, password) are not hardcoded in the script and must be provided manually.

---

## 🚀 How to Run the Project
### 1️⃣ Install Required Dependencies
First, install the dependencies:
```bash
pip install -r requirements.txt
```

### 2️⃣ Run the Jupyter Notebook
```bash
jupyter notebook retail_sales.ipynb
```

---

## 📦 Technologies Used
- **Python** (pandas, SQLAlchemy)
- **PostgreSQL** (local database)
- **Jupyter Notebook** (for documenting the ETL process)

---

## 📌 Possible Extensions
✅ Add SQL-based data analysis.
✅ Visualize results in Tableau / Power BI.
✅ Automate data extraction from an API.


