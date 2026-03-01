# 🧹 Data Cleaning & Preparation – Task 2  
### Data Analyst Internship – SkillCraft Technology  

---

## 👤 Intern Details
**Name:** Raseena R  
**Role:** Data Analyst Intern  
**Duration:** 1 Month Educational Internship  

---

## 📌 Project Overview
This project focuses on cleaning and preparing a real-world retail dataset using Python and Pandas in Google Colab.

The objective was to ensure the dataset is accurate, consistent, and ready for further analysis by handling missing values, correcting data types, and validating records.

---

## 🎯 Objectives
- Load dataset into Python environment  
- Inspect dataset structure and data types  
- Identify and handle missing values  
- Check and remove duplicate records  
- Convert incorrect data types  
- Export cleaned dataset  

---

## 🛠 Tools Used
- Python  
- Pandas  
- Google Colab  

---

## 📂 Dataset Description
**Dataset:** Global Superstore Dataset  

The dataset contains **51,290 rows and 24 columns**, including:

- Order ID  
- Order Date  
- Ship Date  
- Customer Name  
- Segment  
- Country  
- Region  
- Category  
- Sales  
- Profit  
- Discount  
- Shipping Cost  
- Order Priority  

---

## ✅ Tasks Performed

### 1️⃣ Dataset Loading
The dataset was loaded using Pandas with proper encoding.
<img width="1920" height="1080" alt="1" src="https://github.com/user-attachments/assets/82a38579-c888-4cb3-bdd9-94a263b70add" />

### 2️⃣ Dataset Inspection
Used:
- df.head()
- df.info()
- df.shape
Confirmed dataset contains 51,290 records and 24 columns.
<img width="1920" height="1080" alt="2" src="https://github.com/user-attachments/assets/7204c73d-d09e-44e3-b1ec-54313f569a6c" />

### 3️⃣ Handling Missing Values

Checked missing values using:
    df.isnull().sum()

- Found missing values in the Postal Code column.
- Converted Postal Code to object type.
- Replaced missing values with "Unknown"
<img width="1920" height="1080" alt="3" src="https://github.com/user-attachments/assets/f0d654c8-8a50-420e-9bca-16431421170c" />
<img width="1920" height="1080" alt="4" src="https://github.com/user-attachments/assets/b7975408-ee71-4383-9d25-37a5e5a4a894" />
<img width="1920" height="1080" alt="7" src="https://github.com/user-attachments/assets/96493392-054f-414d-b5a3-ce339343ce9e" />


### 4️⃣ Duplicate Record Check

  Checked duplicates using:
      df.duplicated().sum()
- No duplicate records were found.
<img width="1920" height="1080" alt="7" src="https://github.com/user-attachments/assets/5548c829-7866-4cc7-bdb0-9b2b2ef2dd30" />

### 5️⃣ Data Type Conversion

Converted Order Date and Ship Date from object type to datetime format:

  df["Order Date"] = pd.to_datetime(df["Order Date"])
  df["Ship Date"] = pd.to_datetime(df["Ship Date"])

<img width="1920" height="1080" alt="5" src="https://github.com/user-attachments/assets/a839bf92-5326-4894-8f9e-908b39732fa3" />
<img width="1920" height="1080" alt="6" src="https://github.com/user-attachments/assets/e742f234-f1d1-4347-817a-0cdb757ba14d" />

### 6️⃣ Export Cleaned Dataset

Exported cleaned dataset as:

  df.to_csv("Cleaned_Global_Superstore2.csv", index=False)
<img width="1920" height="1080" alt="8" src="https://github.com/user-attachments/assets/b9800652-9a9c-46ff-859e-63deefad4ea4" />

### 📊 Final Dataset Summary

  - Total Rows: 51,290
  - Total Columns: 24
  - No missing values
  - No duplicate records
  - Correct data types assigned
  - Cleaned dataset exported successfully

### 📈 Key Outcomes

- Ensured data consistency and reliability
- Improved dataset quality for further analysis
- Prepared dataset for visualization and dashboard creation
- Strengthened data preprocessing skills

### 🚀 Conclusion

This task demonstrates practical data cleaning and preprocessing skills using Python and Pandas.

The dataset has been successfully cleaned and structured, ensuring accurate and reliable analysis in future tasks.

This reflects real-world data preparation practices required for a Data Analyst role.
