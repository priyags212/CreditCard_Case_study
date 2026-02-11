# 📊 Credit Risk Analysis – Banking Case Study

## 🏦 Project Overview
This project analyzes large-scale banking customer and loan data to identify patterns influencing loan default risk.
Using **Exploratory Data Analysis (EDA)** and **Statistical Hypothesis Testing**, the project uncovers high-risk and low-risk customer segments and provides actionable business recommendations to support data-driven lending decisions.
The analysis is based on the **Home Credit Default Risk dataset**.

## 🎯 Objectives
- Identify key factors associated with loan default  
- Understand demographic and financial risk patterns  
- Perform statistical hypothesis testing  
- Segment customers into high-risk and low-risk groups  
- Provide business recommendations to improve credit risk assessment  

## 🗂 Dataset Information
| Dataset | Records | Description |
|----------|----------|-------------|
| Applicants Data | 307,511 rows × 122 columns | Customer demographic & financial details |
| Previous Loans Data | 1,670,214 rows (cleaned to 69,635) | Historical loan behavior |

## 📥 Dataset Source
The dataset used in this project is the **Home Credit Default Risk dataset** available on Kaggle.
Due to large file size, the dataset is not included in this repository.
You can download it from:
https://www.kaggle.com/competitions/home-credit-default-risk/data

### Data Includes:
- Demographics (Age, Gender, Education)
- Income & Employment Details
- Credit Amount & Annuity
- Loan Purpose
- Contract Status
- Housing Type

## ⚙️ Data Preprocessing
- Removed columns with more than 40% missing values  
- Imputed numerical missing values using median  
- Filled categorical missing values using mode  
- Handled invalid categories (`XNA`, `XAP`)  
- Merged applicant and previous loan datasets  
- Converted negative day values into meaningful age and employment years  

## 🔧 Feature Engineering
- Created **Age in Years** from `DAYS_BIRTH`
- Created **Employment Years** from `DAYS_EMPLOYED`
- Binned income and credit into meaningful ranges
- Defined target variable:
  - `0 → Non-Defaulter`
  - `1 → Defaulter`

## 📊 Exploratory Data Analysis (EDA)

Performed:
- Univariate Analysis  
- Bivariate Analysis  
- Multivariate Analysis
  
Analyzed relationships between:
- Income vs Default Rate  
- Education vs Default Probability  
- Gender vs Default  
- Housing Type vs Risk  
- Loan Purpose vs Default  

Visualizations include:
- Distribution plots  
- Box plots  
- Count plots  
- Correlation analysis  

## 📈 Hypothesis Testing
Statistical testing was conducted to validate key assumptions:
1. Defaulters have significantly lower income than non-defaulters  
2. Default rate differs by gender  
3. Education level impacts default probability  
4. Overall company default rate exceeds 10%  

## 🔍 Key Insights
### 🚨 High-Risk Segments
- Low-income applicants  
- Working income type  
- Loan purpose: Repairs  
- Housing type: Co-op apartments  

### ✅ Low-Risk Segments
- Students  
- Pensioners  
- Businessmen  
- Loan purpose: Education & Business Development  
- Housing: With parents / House / Apartment  

## 📌 Business Recommendations
- Strengthen screening for low-income and working applicants  
- Apply stricter validation for repair-related loans  
- Use previous loan behavior as a strong risk indicator  
- Incorporate income range and occupation into risk scoring models  

## 🛠 Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- SciPy  
- Statsmodels  
- Scikit-learn  
- Jupyter Notebook  

## 📦 Requirements
numpy
pandas
scipy
matplotlib
seaborn
statsmodels
scikit-learn
jupyter

## ▶️ How to Run the Project
### 1️⃣ Clone the repository
```bash
git clone https://github.com/priyags212/CreditCard_Case_study.git
```
### 2️⃣ Navigate to project folder
```bash
cd CreditCard_Case_study
```
### 3️⃣ Install dependencies
```bash
pip install -r requirements.txt
```
### 4️⃣ Open Jupyter Notebook
```bash
jupyter notebook
```
Open `Credit_Case_study.ipynb` and run all cells sequentially.
---

## 🚀 Future Scope
- Build predictive models (Logistic Regression, Random Forest)  
- Create credit risk scoring model  
- Develop interactive dashboard (Power BI / Streamlit)  
- Deploy as end-to-end ML pipeline  

---
## 📌 Conclusion
This project demonstrates how data analytics and statistical techniques can be applied to evaluate credit risk effectively.
The insights support data-driven lending decisions by helping financial institutions:
- Identify high-risk customer segments  
- Improve credit assessment strategies  
- Reduce default exposure  
- Enhance portfolio performance
  
⭐ If you found this project valuable, feel free to connect and collaborate!
