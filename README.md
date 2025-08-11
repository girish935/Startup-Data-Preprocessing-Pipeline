## Startup-Data-Preprocessing-Pipeline
# Startup Data Preprocessing

This project focuses on preprocessing a startup dataset to prepare it for further analysis tasks. The main aim is to clean, transform, and organize the data for better usability.

## Project Overview

- Load the raw startup data into a pandas DataFrame.
- Handle missing values by identifying and filling or removing them.
- Remove duplicate rows to maintain data integrity.
- Convert data types where necessary to ensure consistency.
- Encode categorical variables using techniques like one-hot encoding.
- Drop irrelevant or redundant columns to simplify the dataset.
- Perform final checks to ensure the data is clean and ready for analysis.

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



