*Data Cleaning – Preparing the Dataset for Analysis*

This project focuses on performing a complete data-cleaning workflow to make the dataset suitable for accurate analysis and insight extraction.
The goal was to improve data quality by handling missing values, removing inconsistencies, detecting outliers, and ensuring the dataset is fully analysis-ready.

📌 Project Overview

The data-cleaning process includes:

Dataset exploration

Handling missing values

Duplicate detection

Standardization

Outlier detection & removal using IQR

Preparing the dataset for further analytics

This ensures the dataset is structured, consistent, and ready for advanced analysis or machine learning tasks.

🛠️ Steps Performed

1️⃣ Data Import & Initial Exploration

To understand the dataset, I imported all necessary Python libraries and explored the data using:

head()

info()

data.columns

describe()

isnull().sum()

This helped identify missing values, incorrect data types, and basic summary statistics.

2️⃣ Handling Missing Values

Missing values were handled carefully based on column characteristics:

For numeric column:

reviews_per_month → filled missing values with 0

For text columns:

name → filled with ‘Unknown’

host_name → filled with ‘Unknown’

This step prevents issues during analysis and ensures consistency in the dataset.

3️⃣ Duplicate Record Check

Searched for duplicate entries in the dataset.

No duplicates were found, so no data removal was needed.

4️⃣ Standardization

To maintain uniformity across the dataset, all string columns were converted to lowercase.

This helps avoid treating similar text values as different due to capitalization differences.

5️⃣ Outlier Detection & Removal (IQR Method)

Used the Interquartile Range (IQR) method to identify and remove outliers from numerical columns.

Steps included:

Calculating Q1, Q3, and IQR

Detecting extreme values

Removing rows with outliers

Removing outliers improves accuracy and reliability in future insights and modeling.

✅ Final Output

After completing the cleaning process, the dataset is now:

Clean

Standardized

Free from missing values

Free from outliers

Ready for accurate analysis and visualization

This structured dataset can now be used confidently for EDA, machine learning, and business insights.

🧰 Tech Stack Used

Python,
Pandas,
NumPy,
Matplotlib / Seaborn, 
Google Colab.
