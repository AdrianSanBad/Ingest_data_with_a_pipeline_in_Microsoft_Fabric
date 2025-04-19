# 🚀 Microsoft Fabric - Data Ingestion and Transformation Pipeline

This repository contains a hands-on exercise implementing a full ETL (Extract, Transform, Load) pipeline in **Microsoft Fabric**. It demonstrates how to ingest data from an external HTTP source, transform it using **Apache Spark**, and load it into a **Lakehouse** table in Delta format.

## 📁 Project Structure

The pipeline consists of three main stages:

1. **Delete old files**  
   Clears existing `.csv` files in the `new_data` folder before each run.
2. **Copy sales data**  
   Fetches fresh sales data from an external HTTP URL and stores it as `sales.csv` in the lakehouse.
3. **Load and transform data with Spark notebook**  
   A Spark notebook reads the CSV, adds new columns, filters, and stores the result in a Delta Lake table named `new_sales`.

---

## 🛠 Technologies Used

- Microsoft Fabric (Trial mode)
- Data Pipelines
- Apache Spark Notebooks (PySpark)
- OneLake and Lakehouse storage
- Delta Lake format

---

## 📷 Screenshots

### ✅ Final Pipeline Design

![Final Pipeline](images/pipeline.png)

---

### 📊 Delta Table: `new_sales`

![Delta Table Preview](images/new_sales_table.png)

---

## 📎 Source Data

The source data is a CSV file retrieved from a public GitHub repository:
https://raw.githubusercontent.com/MicrosoftLearning/dp-data/main/sales.csv

## 🧑‍💻 Author
[Adrian Sanchez Badillo]
[https://www.linkedin.com/in/adriansanbad/]

