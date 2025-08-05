## Startup-Outcome-Prediction-Machine-Learning-Pipeline
##  Project Overview
This project aims to **predict the outcome of startups**—whether they will succeed (Operating or IPO) or fail (Acquired or Closed)—using supervised machine learning techniques.  

The process includes:
- Preprocessing a dataset of startup companies
- Feature engineering (e.g., company age)
- Normalization and encoding of data
- Creating a binary target column `Active_Status` to classify startup status (1 = Active, 0 = Not Active)

This project was developed as part of my **Data Science Internship at Technocolabs**.
---
##  Dataset
Due to file size limitations, the dataset is available via Google Drive.
🔗 [Download companies_cleaned.csv]( https://drive.google.com/file/d/1rsWPL2ClXEoBjJ4VOiSia1UDLUfGKGqA/view?usp=sharing )
---

## Key Tasks Performed

-  Extracted `founded_year` from `founded_at`
-  Created `company_age` using: `2025 - founded_year`
-  Scaled numeric features using `MinMaxScaler`:
    - `funding_total_usd`
    - `funding_rounds`
    - `investment_rounds`
    - `company_age`
-  One-hot encoded categorical columns:
    - `category_code`
    - `country_code`
-  Created binary label column `Active_Status`
    - `1` = Active (Operating or IPO)
    - `0` = Not Active (Acquired or Closed)
-  Final cleaned dataset saved as `processed_companies_dataset.csv`

---

## Project Structure

Startup-Outcome-Prediction-ML/

── data/                            # Raw dataset (Compaines.csv)
── processed_companies_dataset.csv  # Cleaned and preprocessed dataset
── notebooks/                       # (if applicable)
── README.md                        # Project documentation
── requirements.txt                 # Python dependencies
── your_script.py / .ipynb          # Main analysis code

---

##  Variable Dictionary

| Variable Name         | Description                                |
|-----------------------|--------------------------------------------|
| `name`                | Name of the startup                        |
| `category_code`       | Industry of the startup                    |
| `status`              | Business status (operating, acquired...)   |
| `founded_at`          | Foundation date                            |
| `founded_year`        | Extracted year from `founded_at`           |
| `company_age`         | Company age (2025 - founded_year)          |
| `country_code`        | Country of origin                          |
| `investment_rounds`   | Number of investment rounds                |
| `funding_total_usd`   | Total funding received in USD              |
| `funding_rounds`      | Number of funding rounds                   |
| `Active_Status`       | Final label column (1 = Active, 0 = Not)   |

## 🧪 Model Building

Model building not included in this part, but the dataset is now ready for supervised learning models such as Logistic Regression, Random Forest, or XGBoost.

---

##  Setup Instructions

### 1. Clone the repository

## bash
git clone https://github.com/girish935/Startup-Outcome-Prediction-ML.git
cd Startup-Outcome-Prediction-ML

### 2. Install dependencies

## bash
pip install -r requirements.txt

### 3. Run preprocessing script

## bash
python script.py  # Or open your Jupyter Notebook

## 📈 Output

Processed dataset saved as: `Startup_cleaned_data.csv`  
Use this file for ML modeling.






