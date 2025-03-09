# Fraudulence Detection Using Machine Learning

## Overview
This project focuses on detecting fraudulent transactions in online marketplaces using **Machine Learning (ML) techniques**. With the increasing rate of cyber fraud, advanced detection methods are necessary to safeguard users and businesses from financial losses.

## Problem Statement
As online transactions grow, so do fraudulent activities, leading to significant financial damage and loss of consumer trust. Traditional fraud detection methods often fail to keep up with evolving fraud techniques. This project explores how **ML algorithms** can enhance fraud detection by analyzing transaction patterns and identifying suspicious activities.

## Dataset
- **Size:** 151,112 rows and 10 columns
- **Features:** Includes user details (age, sex), transaction details (purchase time, value), and technical data (IP address, browser used).
- **Target Variable:** 'Class' indicating whether a transaction is fraudulent ('1') or not ('0').

## Approach
### 1. **Data Preprocessing**
- Checked for missing values and handled inconsistencies.
- Converted timestamps to useful features such as `signup_hour`, `purchase_day`, and `time_diff`.
- Standardized numerical values for better model performance.

### 2. **Exploratory Data Analysis (EDA)**
- Identified trends and correlations in fraudulent transactions.
- Visualized data distribution to detect anomalies.

### 3. **Machine Learning Models Used**
- **Logistic Regression:** Used as a baseline model but struggled with fraud detection.
- **Random Forest:** Achieved better accuracy, recall, and precision in detecting fraudulent transactions.

### 4. **Results & Model Comparison**
| Model              | Precision | Recall | F1 Score |
|-------------------|------------|------------|------------|
| Logistic Regression | 0% (for fraud cases) | 0% | Low |
| Random Forest      | High | High | Best Performance |

- **Random Forest outperformed Logistic Regression**, making it the preferred model for fraud detection.

## Key Takeaways
✅ **Effective Fraud Detection** – ML models successfully identified fraudulent transactions.
✅ **Random Forest Performed Best** – Achieved high accuracy and recall.
✅ **Future Work** – Further tuning the model and testing on real-time transactions.

## Technologies Used
- **Machine Learning:** Logistic Regression, Random Forest
- **Programming Language:** Python (Pandas, NumPy, Scikit-Learn)
- **Data Analysis & Visualization:** Matplotlib, Seaborn
- **Data Processing:** Feature Engineering, Standardization

## How to Run the Project
### 1. Clone the Repository
```bash
git clone https://github.com/Neelimavanukuri/fraud-detection-ml
cd fraud-detection-ml
```
### 2. Install Dependencies
```bash
pip install -r requirements.txt
```
### 3. Run the Jupyter Notebook
```bash
jupyter notebook
```
Open `Fraudulence Detection Using ML.ipynb` and execute the cells.

