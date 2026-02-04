# ML_CA1_Exploratory_Data_Analysis
Using the house price data set, i completed steps 1 through 3 of the EDA process. 
# CA01 – Exploratory Data Analysis & Data Preparation (House Price Dataset)

##  Project Overview
This project focuses on **Exploratory Data Analysis (EDA)** and **data preparation** for a house price dataset.  
The objective is to analyze the dataset structure, identify data quality issues, clean the data, and prepare it to be **analytics-ready** for future machine learning models.

 **Model building is NOT part of this project.**

---

##  Dataset
The dataset is provided as part of the course materials:

- **Training Data:** `house-price-train.csv`
- **Source:**  
  https://github.com/ArinB/MSBA-CA-Data/tree/main/CA01

Only the **training dataset** is used for this assignment.

---

##  Project Goals
1. Understand the structure and characteristics of the dataset  
2. Identify data quality issues using EDA  
3. Fix data quality issues using Python  
4. Analyze feature collinearity and perform feature selection  

---

##  Project Structure
├── CA01_EDA_House_Price.ipynb
└── README.md

All analysis, visualizations, explanations, and conclusions are contained within the notebook.

---

##  Part 1 – Data Understanding & Exploratory Data Analysis (EDA)

**Key steps:**
- Loaded and inspected dataset structure
- Identified numeric and categorical variables
- Performed univariate analysis:
  - Histograms and boxplots for numeric features
  - Frequency analysis and bar charts for categorical features
- Performed bivariate analysis:
  - Numeric features vs. target (`SalePrice`)
  - Categorical features vs. target
- Generated a correlation heatmap
- Created a **Data Quality Report** identifying:
  - Missing values
  - Potential outliers
  - Duplicate rows
  - ID-like columns
  - Zero or near-zero variance features

---

##  Part 2 – Data Cleaning & Pre-Processing

**Data quality issues identified in Part 1 were fixed using the following techniques:**

- Removed duplicate rows
- Dropped columns with excessive missing values
- Imputed missing values:
  - Numeric features → median
  - Categorical features → `"Unknown"`
- Handled outliers using **IQR-based capping**
- Removed ID-like columns
- One-hot encoded categorical variables
- Preserved the target variable (`SalePrice`) separately

The result is a **clean, encoded, analytics-ready dataset**.

---

## 🔗 Part 3 – Collinearity Analysis & Feature Selection

 **Only collinearity and feature selection were performed (no class imbalance analysis).**

**Steps included:**
- Computed correlation matrix for numeric features
- Visualized correlations using heatmaps
- Identified highly correlated feature pairs (|correlation| ≥ 0.90)
- Dropped redundant features based on weaker correlation with the target variable
- Produced a final feature-selected dataset

---

## 🛠️ Tools & Libraries Used
- Python
- pandas
- numpy
- matplotlib
- seaborn

---

##  Final Output
- A fully documented Jupyter Notebook
- Cleaned and feature-selected dataset ready for future machine learning models
- No model training or evaluation included

---

## 📝Notes
- All observations, explanations, and conclusions are included in the notebook
- This project follows the CA01 assignment instructions exactly

---

## 👤 Author
**Jessica Thai**  
MSBA – Exploratory Data Analysis  
