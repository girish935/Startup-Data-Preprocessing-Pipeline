## Startup-Data-Preprocessing-Pipeline
# Startup Data Preprocessing :- Project Overview

This project focuses on preprocessing startup data to prepare it for Exploratory Data Analysis (EDA) and further machine learning applications.
The dataset contains 7,326 rows and 30 features, including numerical, categorical, and boolean columns related to startup performance, funding, milestones, and geographical details.
The preprocessing steps ensure data quality, consistency, and readiness for analysis.

## Key Steps

1. **Data Loading**  
   Loading the dataset into pandas from CSV or Excel file.

2. **Data Cleaning**  
   - Checking for missing or null values.  
   - Filling or removing missing data appropriately.  
   - Removing duplicate records.

3. **Data Transformation**  
   - Encoding categorical features (`category_code`) with one-hot encoding.  
   - Changing boolean columns from `True/False` to `0/1` for numeric consistency.  
   - Dropping unwanted columns such as `closed_at`.

4. **Saving Processed Data**  
   The cleaned and preprocessed data is saved into a new Excel or CSV file for further use.

## Toole Used

- Python 3.x  
- Pandas library for data manipulation  
- Jupyter Notebook for interactive coding and documentation

## How to Run

1. Clone the repository or download the notebook file.
2. Open the notebook in Jupyter Notebook or JupyterLab.
3. Run the cells sequentially to preprocess the startup dataset.
4. The processed data will be saved as `cleaned_startup_data_processed.xlsx` or `cleaned_startup_data_processed.csv`.

## Notes

- Ensure have you the required dependencies installed:  
  ```bash
  pip install pandas openpyxl

Conclusion :- The dataset has been thoroughly cleaned and preprocessed to ensure accuracy and consistency. New features and labels were added to help build effective predictive models in the future. This preprocessing step lays a strong foundation for successful startup status prediction.



