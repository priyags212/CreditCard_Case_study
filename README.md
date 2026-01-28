# 📊 Credit Risk Analysis – Banking Case Study

## 📌 Project Overview
This project focuses on analyzing banking customer and loan data to identify patterns that influence loan default risk. Using data analytics and statistical techniques, the project uncovers high-risk and low-risk customer segments and provides actionable insights to support data-driven lending decisions.

The analysis is based on the **Home Credit Default Risk dataset** and involves data cleaning, exploratory data analysis (EDA), feature engineering, hypothesis testing, and business recommendations.

## 🎯 Objectives
- Identify key factors associated with loan default
- Understand customer behavior and risk patterns
- Perform statistical hypothesis testing
- Provide recommendations for improving credit risk assessment

## 🗂 Dataset Information
- **Applicants Dataset:** 307,511 rows, 122 columns  
- **Previous Loans Dataset:** 1,670,214 rows (cleaned to 69,635 rows)

Data includes:
- Demographics  
- Income & employment details  
- Credit & annuity values  
- Loan purpose & contract status  

## ⚙️ Data Preprocessing
- Removed columns with more than 40% missing values  
- Imputed numerical missing values using median  
- Filled categorical missing values using mode  
- Handled invalid values such as `XNA` and `XAP`  
- Merged applicant and previous loan datasets  

## 🔧 Feature Engineering
- Age in years from DAYS_BIRTH  
- Employment years from DAYS_EMPLOYED  
- Binning income and credit into ranges  
- Target variable:
  - `0` → Non-defaulter  
  - `1` → Defaulter  

## 📊 Exploratory Data Analysis (EDA)
- Univariate, bivariate, and multivariate analysis  
- Box plots and distributions for income, credit, and annuity  
- Relationship between education, income, gender, housing type, and default  

## 📈 Hypothesis Testing
- Defaulters have lower income than non-defaulters  
- Default rate differs by gender  
- Education level impacts default probability  
- Overall company default rate is greater than 10%  

## 🔍 Key Insights
**High-Risk Groups**
- Low income applicants  
- Working income type  
- Loan purpose: Repairs  
- Housing type: Co-op apartments  

**Low-Risk Groups**
- Students, Pensioners, Businessmen  
- Loan purpose: Education, Business Development  
- Housing: With parents, House/Apartment  

## ✅ Business Recommendations
- Strengthen screening for low-income and working applicants  
- Avoid risky loan purposes such as repairs  
- Use previous loan behavior as a key risk indicator  
- Build predictive models using income, credit range, occupation, and education  

## 🛠 Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- SciPy  
- Jupyter Notebook  
- SQLite  

## ▶️ How to Run the Project
1. Clone the repository  
   ```bash
   git clone https://github.com/priyags212/Credit-Risk-Analysis-Banking-Case-Study.git
2. Open the notebook in Jupyter Notebook

3. Run cells sequentially
   
📌 Conclusion
This project demonstrates how data analytics and statistics can be used to evaluate credit risk and support smarter lending decisions. The findings help banks reduce default rates and improve portfolio quality.
