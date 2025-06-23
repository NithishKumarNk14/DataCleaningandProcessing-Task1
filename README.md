# DataCleaningandProcessing-Task1
# 🧹 Marketing Campaign Data Cleaning Project

This project involves cleaning, preprocessing, and preparing the `marketing_campaign.csv` dataset for analysis and machine learning tasks.

---

## 📁 Dataset Description

The dataset contains customer demographic and behavioral data for a marketing campaign, including:

- Personal info: `ID`, `Year_Birth`, `Education`, `Marital_Status`, `Income`
- Purchase behavior: `MntWines`, `MntFruits`, `MntMeatProducts`, etc.
- Campaign responses: `AcceptedCmp1` to `AcceptedCmp5`, `Response`
- Website activity: `NumWebPurchases`, `NumWebVisitsMonth`
- Customer registration date: `Dt_Customer`

---

Cleaning Tasks Performed

| ✅ Load CSV | Loaded the dataset using tab (`\t`) separator |
| ✅ Handle Missing Values | Removed rows with missing `Income` |
| ✅ Remove Duplicates | Used `.drop_duplicates()` to remove redundant entries |
| ✅ Standardize Text Columns | Lowercased and stripped whitespaces in `education` and `marital_status` |
| ✅ Convert Dates | Parsed `Dt_Customer` to `datetime` format |
| ✅ Rename Columns | Made all column names lowercase with underscores |
| ✅ Fix Data Types | Ensured numeric columns are integers/floats, and date is proper `datetime` |
| ✅ Derived Columns | Created `age` from `Year_Birth` |

---

 Files

- `marketing_campaign.csv` — Original raw dataset (tab-separated)
- `cleaned_marketing_analysis.csv` — Cleaned version of the dataset (generated)
- `task1_cleaningandprocessing (1)` — python script to perform cleaning and processing work
- `README.md` — Project documentation

---

How to Run

1. Upload `marketing_campaign.csv` in your Colab environment
2. Run the notebook `clean_data_script.ipynb`
3. The cleaned data will be saved as `cleaned_marketing_analysis.csv`
4. Optionally, download it using:
   ```python
   from google.colab import files
   files.download('cleaned_marketing_analysis.csv')
