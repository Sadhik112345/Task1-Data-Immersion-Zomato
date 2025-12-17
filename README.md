# 🍽️ Data Immersion & Wrangling – Zomato Dataset

**Internship:** Data Analytics Internship – ApexPlanet Software Pvt. Ltd.
**Task:** Task 1 – Data Immersion & Wrangling
**Duration:** 10 Days

---

## 📌 Objective

The objective of this task is to gain a deep understanding of the dataset and perform the critical first step of data analysis: **data acquisition, quality assessment, cleaning, transformation, and preparation** to produce an analysis-ready dataset.

---

## 📊 Dataset Description

* **Dataset Name:** Zomato Raw Restaurant Data
* **Source:** Open-source dataset (used due to unavailability of an official dataset)
* **Description:**
  The dataset contains restaurant-level information such as online ordering availability, table booking options, customer ratings, votes, approximate cost for two people, and restaurant category/type.

Each row represents a single restaurant listed on Zomato.

---

## 🧾 Data Dictionary

A detailed **data dictionary** was created to understand each column’s:

* Meaning
* Data type
* Example values
* Business relevance

📁 File: `data_dictionary.xlsx`

---

## 🔍 Data Quality Assessment

The following data quality issues were identified in the raw dataset:

* Missing and invalid values in the `rate` column (e.g., "NEW", "-")
* Incorrect data types (ratings stored as text)
* Duplicate records
* Inconsistent formatting in categorical columns
* Numeric columns stored as strings (cost values with commas)

---

## 🧹 Data Cleaning & Transformation

Using **Python (Pandas)**, the following steps were performed:

* Removed duplicate records
* Handled missing values using median imputation
* Cleaned and converted ratings to numeric format
* Standardized categorical text fields
* Converted `online_order` and `book_table` from text to Boolean
* Cleaned and converted cost column to numeric
* Created a new feature: `Cost_Category` (Low / Medium / High)

📁 File: `data_cleaning.py`

---

## 🧠 Feature Engineering

A new categorical feature was created:

* **Cost_Category** – Segments restaurants based on approximate cost for two people using value-based binning.

---

## 📦 Final Output

The final output is a **clean, structured, and analysis-ready dataset**.

📁 File: `cleaned_zomato_data.csv`

---

## 🛠️ Tools & Technologies Used

* Python
* Pandas
* NumPy
* Jupyter Notebook / VS Code
* GitHub

---

## 📁 Repository Structure

```
Task1-Data-Immersion-Zomato/
│
├── data_dictionary.xlsx
├── data_cleaning.py
├── cleaned_zomato_data.csv
├── README.md
```

---

## 🎥 Task Submission

* A **3–5 minute LinkedIn video** was created explaining:

  * Dataset overview
  * Data quality issues
  * Cleaning and transformation steps
  * Final cleaned dataset

* The task was submitted through the **ApexPlanet Internship Portal** with:

  * GitHub repository link
  * LinkedIn video link

---

## ✅ Conclusion

This task strengthened my understanding of real-world data issues and enhanced my skills in data preprocessing, cleaning, and feature engineering. The resulting dataset is ready for exploratory data analysis and business insights in subsequent tasks.

---
