# Task-1-Data-Cleaning-and-Preprocessing-Of-Netflix-Movies-and-TV-Shows

# Netflix Dataset - Data Cleaning and Preprocessing

## 📌 Objective
To clean and prepare a raw Netflix dataset by handling missing values, removing duplicates, and ensuring consistency in formatting and data types.

---

## 🛠️ Tools And Programming Language Used
- Python
- Pandas
- Jupyter Notebook

---

## 📂 Dataset Overview
Original dataset contains:
- **8807** rows
- **12** columns
- Columns with missing values: `director`, `cast`, `country`, `date_added`, `rating`, `duration`

---

## 🔧 Steps Performed

### 1. **Identified and Handled Missing Values**
- Used `.isnull().sum()` to find missing values.
- Filled missing values in `director`, `cast`, and `country` columns with `'Unknown'`.
- Dropped rows where `date_added`, `rating`, or `duration` were missing using `dropna()`.

### 2. **Removed Duplicates**
- Used `.duplicated().sum()` to check for duplicate rows.
- Removed duplicates using `.drop_duplicates()`.

### 3. *(Optional Additional Steps — if included)*
- Standardized text values (`type`, `rating`, `country`) to consistent format using `.str.strip().str.title()`.
- Converted `date_added` to datetime format using `pd.to_datetime()`.
- Renamed all column headers to lowercase and replaced spaces with underscores.
- Verified and corrected data types.

---

## ✅ Output
- Cleaned dataset saved as: `netflix_dataset_cleaned.csv`
- All missing values handled and duplicates removed.

---

## 📄 Summary of Changes
- Rows after cleaning: *[final row count]*  
- Columns cleaned: `director`, `cast`, `country`, `date_added`, `rating`, `duration`  
- Duplicates removed: *[number of duplicates]*  
- Date format standardized: `dd-mm-yyyy`

---

## 📁 Files Included
- `netflix_dataset.csv` – Raw dataset
- `netflix_dataset_cleaned.csv` – Cleaned dataset
- `Netflix Movies and TV Shows Dataset.ipynb` – Jupyter Notebook with all code
- `README.md` – This file

---

## 👨‍💻 Author
Surjeetsinh Nandkumar Thakur  

