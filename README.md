# E-Commerce Data Cleaning and Transformation using NumPy and Pandas
A production style data preprocessing pipeline built on a real-world messy e-commerce dataset. Transforming raw, inconsistent data into analytics ready output using Python and and its libraries : NumPy and Pandas. 

> Production-style data preprocessing pipeline on a real-world
> messy e-commerce dataset of 1200 records cleaned and transformed
> into analytics ready output using Python, NumPy and Pandas.

---

## Project Overview

Raw data from real systems is never clean. This project simulates
that reality — starting with a messy dataset of 1200 orders
containing nulls, duplicates, mixed formats, dirty strings and
wrong data types and transforms it into structured output.

---

## Project Structure

ecommerce-data-cleaning/
 ┣ ecommerce_dataset.csv                    ← Raw dataset
 ┣ Ecommerce_Data_Cleaning_Pandas.ipynb    ← Core cleaning
 ┣ Data_Cleaning_and_transformation.ipynb  ← EDA + transforms
 ┗ README.md

---

## Dataset Overview

| Feature  | Details                                        |
|----------|------------------------------------------------|
| Records  | 1,200 rows                                     |
| Columns  | 11 (Order_ID, Customer_Name, Email, etc.)      |
| Issues   | Nulls, duplicates, mixed dates, bad dtypes     |

---

##  Before vs After Cleaning

| Column           | Before                        | After                    |
|------------------|-------------------------------|--------------------------|
| Customer_Name    | Amit$, Rahul@, NaN            | Amit, Rahul, Guest       |
| Quantity         | "five", "two", NaN            | 5, 2, mean value         |
| Unit_Price       | "$199.99" (string)            | 199.99 (float)           |
| Order_Date       | 01/14/2023 & 30-07-2023       | Uniform datetime format  |
| Product_Category | "elec", "electronic"          | "electronics"            |

---

## Techniques Applied :

- Null handling — fillna() with contextual values & mean imputation
- Duplicate removal — drop_duplicates()
- Regex cleaning — stripped special chars from names & IDs
- Type casting — strings to float, dates to datetime
- Word-to-number mapping — "five" → 5
- Category standardization — mapped inconsistent labels
- Feature engineering — Total_Amount, Order_Year, Price_Category

---

# Tech Stack :

Python 3.14.5 | Pandas | NumPy | Jupyter Notebook

---

# How to Run :
git clone https://github.com/Radhikaa2808/Data-Cleaning-and-EDA.git
cd Data-Cleaning-and-EDA
pip install pandas numpy jupyter
jupyter notebook

## Author :

Radhika Pal | BCA in  Data Science & AI | Shri Ramswaroop Memorial University, Lucknow.
