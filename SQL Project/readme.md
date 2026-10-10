# 🏥 Healthcare Data Analysis Using SQL

## 📌 Project Overview

This project focuses on preparing and converting a healthcare dataset into an **SQL-ready format** for database analysis.

The project uses a healthcare master dataset containing patient and healthcare-related information. Using **Python and Pandas**, I cleaned and standardized the dataset structure and generated SQL `INSERT` statements that can be used to load the data into a relational database for further analysis.

The project demonstrates my understanding of **data preparation, SQL database loading, structured healthcare data, and data analytics workflows**.

---

## 🎯 Project Objectives

The main objectives of this project were to:

* Prepare healthcare data for SQL-based analysis.
* Standardize column names for database compatibility.
* Handle spaces, dots, and special characters in column names.
* Convert the healthcare dataset into SQL `INSERT` statements.
* Create a reusable SQL file for loading healthcare records into a database.
* Build a foundation for further healthcare data analysis using SQL.

---

## 🛠️ Tools & Technologies

* **SQL** – Database structure and data loading
* **Python** – Data preparation and SQL generation
* **Pandas** – Data manipulation and transformation
* **Jupyter Notebook / Google Colab** – Development environment
* **CSV** – Source healthcare dataset

---

## 🔄 Project Workflow

### 1. Load the Healthcare Dataset

The healthcare master dataset was imported into Python using Pandas.

```python
import pandas as pd

df = pd.read_csv("healthcare mastertable.csv")
```

### 2. Data Preparation

To make the dataset more suitable for SQL/database use, column names were standardized by replacing:

* Spaces with underscores
* Dots with underscores
* Slashes with underscores

```python
df.columns = df.columns.str.replace(" ", "_")
df.columns = df.columns.str.replace(".", "_")
df.columns = df.columns.str.replace("/", "_")
```

This creates cleaner and more database-friendly column names.

### 3. Convert Data into SQL Statements

Each row of the healthcare dataset was converted into an SQL `INSERT` statement.

```python
with open("healthcare_data.sql", "w") as f:
    for _, row in df.iterrows():
        values = "', '".join(str(x).replace("'", "") for x in row)
        f.write(
            f"INSERT INTO healthcare_master VALUES ('{values}');\n"
        )
```

This generated a separate SQL statement for each healthcare record.

### 4. Generate the SQL File

The final SQL file was generated as:

`healthcare_data.sql`

This file can be used to populate a healthcare database table and serve as the starting point for SQL-based analysis.

---

## 📊 Data Analysis Scope

Once loaded into a database, the healthcare dataset can be analyzed to explore areas such as:

* Patient information
* Doctor and healthcare provider information
* Diagnosis patterns
* Treatment information
* Medication records
* Patient visits
* Healthcare trends
* Follow-up requirements
* Patient demographics

These analyses can help transform raw healthcare records into meaningful insights for healthcare decision-making.

---

## 💡 Key Learning Outcomes

Through this project, I gained practical experience in:

* Preparing real-world healthcare data
* Working with Pandas DataFrames
* Standardizing database column names
* Converting structured data into SQL statements
* Understanding SQL data-loading workflows
* Working with healthcare datasets
* Building a foundation for SQL-based data analysis

---

## 📂 Project Structure

```text
Healthcare-SQL-Project/
│
├── Axon_healthcare.ipynb
├── healthcare_data.sql
├── healthcare mastertable.csv
└── README.md
```

---

## 🚀 Future Improvements

The next stage of this project can include writing SQL queries to perform:

* Patient and doctor analysis
* Diagnosis frequency analysis
* Doctor workload analysis
* Monthly healthcare trends
* Follow-up analysis
* Treatment and medication analysis
* Advanced SQL analysis using `JOIN`, `GROUP BY`, subqueries, CTEs, and window functions

---

## 📌 Conclusion

This project demonstrates my ability to take a raw healthcare dataset, prepare it using Python and Pandas, and transform it into an **SQL-ready database format**.

It represents an important step in my **Data Analyst learning journey**, combining data preparation, SQL, Python, and healthcare analytics.

### 🔧 Skills Demonstrated

**SQL | Python | Pandas | Data Cleaning | Data Preparation | Database Management | Healthcare Analytics | Data Analysis**

