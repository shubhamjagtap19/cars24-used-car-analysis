# 🚗 Cars24 Used Car Price Analysis & Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange)
![Matplotlib](https://img.shields.io/badge/Visualization-Matplotlib%2FSeaborn-success)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📌 1. Project Overview
The pre-owned car market in India has grown exponentially, driven by digital platforms like Cars24. However, pricing a used car accurately is complex due to fluctuating depreciation rates, brand positioning, fuel types, and regional demand. 

This project explores the **Cars24 used car dataset** to clean messy real-world data, perform rigorous Exploratory Data Analysis (EDA), engineer predictive features, and uncover key pricing drivers to help buyers and sellers make data-driven decisions.

## 💼 2. Business Problem
Buyers often overpay for used vehicles due to a lack of transparent pricing benchmarks, while sellers struggle to list cars at competitive prices that ensure fast turnover. 
* **The Core Challenge:** How can we accurately determine the fair market value of a pre-owned car based on its attributes (age, kilometers driven, fuel type, transmission, etc.)?

## 🎯 3. Objective
* Clean and preprocess raw transactional car data to handle missing values and anomalies.
* Analyze market trends to identify which factors heavily influence used car depreciation and resale prices.
* Engineer relevant features to optimize datasets for future machine-learning price-prediction models.
* Provide actionable insights for pre-owned automotive marketplaces.

## 📂 4. Dataset
* **Source:** Cars24 pre-owned car listings (`train-cars24-car-price.csv`).
* **Rows & Columns:** Contains transactional attributes detailing car specifications, mileage, manufacturing year, ownership history, and asking prices.

## 🛠️ 5. Tools & Technologies
* **Language:** Python 
* **Libraries for Data Manipulation:** Pandas, NumPy
* **Libraries for Data Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / Google Colab
* **Version Control:** Git & GitHub

## 🧹 6. Data Cleaning & Preprocessing
Real-world data is messy. The data cleaning pipeline handled:
* **Missing Value Treatment:** Identified null values in critical columns and imputed or dropped them logically.
* **Duplicate Removal:** Checked and cleared redundant rows to prevent model bias.
* **Data Type Correction:** Converted text-based numerical columns (like mileage or engine capacity) into proper integer/float data types by stripping units (e.g., "kmpl", "CC").
* **Outlier Detection:** Used Interquartile Range (IQR) and visual boxplots to spot and manage extreme outlier values in selling prices and kilometers driven.

## 📊 7. Exploratory Data Analysis (EDA)
Key questions answered during the analysis phase:
* *How does car age impact resale price?* (Mapped depreciation curves).
* *Do diesel cars hold their value better than petrol cars?* (Compared fuel-type pricing distributions).
* *What is the relationship between kilometers driven and market depreciation?*
* Correlation heatmaps were generated to check multi-collinearity among numerical variables.

## ⚙️ 8. Feature Engineering
To maximize predictive capability, new features were derived from existing data fields:
* **Car Age:** Calculated dynamically from the manufacturing/registration year to current operating age.
* **Brand Extraction:** Separated manufacturer names from vehicle model titles for high-level brand value grouping.
* **Categorical Encoding:** Prepared categorical variables (Transmission, Fuel Type, Ownership) for potential machine learning integration.

## 💡 9. Key Insights
1. **Depreciation Cliff:** Cars lose roughly 40-50% of their initial showroom value within the first 3 years, after which the depreciation curve flattens significantly.
2. **Kilometer Impact:** High mileage heavily penalizes resale value, but reliable brand names (e.g., Maruti, Hyundai) show stronger resilience against high odometer readings.
3. **Transmission Premium:** Automatic transmission variants maintain a noticeably higher resale value margin compared to manual counterparts across identical age brackets.

## 🚀 10. How to Run the Project Locally

Follow these simple steps to run the analysis on your machine:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/shubhamjagtap19/cars24-used-car-analysis.git](https://github.com/shubhamjagtap19/cars24-used-car-analysis.git)
