# 📊 Swiggy Sales Analytics

A data analysis project based on one year of Swiggy sales data. The project focuses on cleaning a real-world sales dataset and extracting meaningful business insights using Python and Pandas.

---

## 📌 Project Overview

The objective of this project is to understand how raw sales data can be cleaned, processed, and analyzed to answer business-related questions.

The project is divided into two major sections:

1. **Data Cleaning – Clean the Dirty Dataset**
2. **E-Commerce Sales Analytics**

A total of **9 questions** are addressed in this project.

The complete implementation and analysis are available in the Jupyter Notebook:

**`Swiggy_Sales_Analysis.ipynb`**

---

# 📂 Dataset

### Dataset Name

**Swiggy Sales Dataset – 1 Year**

### File

`swiggy_sales_1_year.csv`

### Dataset Features

The dataset contains information related to:

- Order Date
- Order ID
- Item Name
- Category
- Quantity
- Item Price
- Discount
- GST
- Delivery Charges
- Customer Paid Amount
- Net Sales
- Payment Method
- Order Status

A Revenue field is derived from the sales information for performing revenue-based analysis.

---

# 🧹 Part 1: Clean the Dirty Dataset

This section focuses on identifying and handling common data-quality problems.

---

## Q1. Missing Values

### Question

**Identify and handle missing values in the dataset, especially blank Price or Quantity values.**

### Answer

The dataset was checked for missing or blank values in all columns.

**Result:**  
No missing values were found in the dataset.

Therefore, no missing-value replacement or removal was required.

### Status

✅ No missing values found

---

## Q2. Duplicate Records

### Question

**Identify duplicate records where the same order or record appears more than once.**

### Answer

The dataset was examined for duplicate records.

Duplicate records can affect the accuracy of sales calculations because the same transaction may be counted more than once.

**Result:**  
Duplicate records were checked and handled during the data-cleaning process.

### Status

✅ Duplicate records checked

---

## Q3. Incorrect Data Types

### Question

**Identify columns where dates, prices, or quantities are stored in an incorrect data type and convert them into appropriate formats.**

### Answer

The data types of important columns were examined and corrected where necessary.

- Date values were converted into an appropriate date format.
- Item Price values were converted into numeric format.
- Quantity values were converted into numeric format.

This ensures that the dataset can be used correctly for calculations and analysis.

### Status

✅ Data types checked and corrected

---

## Q4. Inconsistent Categories

### Question

**Identify inconsistent category names such as `electronics` and `Electronics` and standardize them.**

### Answer

Category values were checked for differences in capitalization and unnecessary spaces.

The category names were standardized into a consistent format.

For example:

- `electronics`
- `Electronics`
- ` electronics `

are treated consistently after cleaning.

### Status

✅ Category values standardized

---

## Q5. Abnormal Values

### Question

**Identify abnormal values such as negative prices or Quantity equal to zero.**

### Answer

The dataset was checked for:

- Negative item prices
- Zero quantities
- Other invalid sales-related values

**Result:**  
No negative item prices or zero-quantity records were found.

Therefore, no abnormal records needed to be removed for these conditions.

### Status

✅ No abnormal price or quantity values found

---
---

# 📁 Project Structure

```text
Swiggy-Sales-Analysis/
│
├── Swiggy_Sales_Analysis.ipynb
├── swiggy_sales_1_year.csv
└── README.md