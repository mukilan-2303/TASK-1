# 📊 Netflix Data Cleaning and Preprocessing

This repository contains a cleaned version of the **Netflix Movies and TV Shows dataset** from Kaggle. The project focuses on essential data cleaning techniques using **Python (Pandas)** to prepare the data for further analysis or machine learning tasks.

---

## 🧹 Task Overview

**Objective:**  
Clean and prepare a raw dataset containing nulls, duplicates, inconsistent text formats, and mixed data types.

**Dataset Source:**  
[Netflix Movies and TV Shows on Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)

---

## 🧰 Tools Used

- Python 3
- Pandas
- Jupyter Notebook (or any Python IDE)

---

## ✅ Cleaning Steps Performed

1. **Loaded the Dataset**  
   Used `pandas.read_csv()` to load the raw CSV.

2. **Exploratory Checks**  
   Used `.info()`, `.describe()`, and `.isnull()` to understand data quality.

3. **Handled Missing Values**  
   - Replaced missing values in `director`, `cast`, and `country` with placeholder values.
   - Forward-filled missing dates in `date_added`.

4. **Removed Duplicates**  
   Removed exact duplicate rows using `.drop_duplicates()`.

5. **Standardized Text**  
   - Converted string columns (e.g., `type`, `country`) to lowercase.
   - Stripped extra spaces.

6. **Date Conversion**  
   Converted `date_added` to datetime format (`YYYY-MM-DD`).

7. **Renamed Columns**  
   Made column names lowercase and replaced spaces with underscores.

8. **Fixed Data Types**  
   - Ensured `release_year` is integer.
   - Verified all date fields are in `datetime` format.

---

## 📁 Files

| File Name                     | Description                              |
|------------------------------|------------------------------------------|
| `netflix_titles.csv`         | Original raw dataset from Kaggle         |
| `netflix_titles_cleaned.csv` | Cleaned dataset (ready for analysis)     |
| `netflix_cleaning.ipynb`     | Jupyter Notebook with all cleaning steps |
| `README.md`                  | Project documentation                    |

---

## 📝 Summary of Changes

- Removed: **X** duplicate rows
- Filled: Missing values in `director`, `cast`, `country`, and `date_added`
- Standardized: Text values in key categorical columns
- Converted: `date_added` to datetime
- Renamed: All columns to snake_case format

---

## 📌 Future Improvements

- Add visualizations for missing data
- Use data profiling tools like `pandas-profiling`
- Extend this for analysis or prediction models

---

## 📬 Contact

Feel free to reach out if you have questions or ideas!

---

**⭐️ Don't forget to star the repo if you found it helpful!**

