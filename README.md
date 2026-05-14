# 📊 Loan Default Risk Analysis — Power BI Dashboard

## 📌 Project Overview

This Power BI project analyzes a Loan Default Dataset to identify 
borrower risk patterns, default behavior, and financial profiles 
across different demographics and employment types.

The dashboard helps financial analysts and risk teams understand 
which borrower segments are most likely to default and why — 
enabling smarter lending decisions.

---

## 💼 Business Problem

Financial institutions lose billions annually due to loan defaults. 
The core question this project answers:

"Which borrower profiles carry the highest default risk, 
and how has that risk changed over time?"

---

## 📄 Dashboard Pages

### Page 1 — Loan Default & Overview
- Loan Amount by Purpose (Home, Business, Education, Auto, Other)
- Average Income by Employment Type
- Default Rate (%) by Employment Type
- Average Loan Amount by Age Group
- Default Rate (%) by Year (2013–2018)

### Page 2 — Applicant Demographics & Financial Profile
- Median Loan Amount by Credit Score Category
- Average Loan Amount by Age Group and Marital Status
- Total Loan (Adults) by Credit Score Bins
- Loan for Middle Age Adults by Mortgage and Dependents
- Number of Loans by Education and Employment Type

### Page 3 — Financial Risk Matrix
- YOY Loan Amount Change by Year
- YOY Default Loans Change by Year
- YTD Loan Amount by Credit Score Bins and Marital Status
- Income Bracket to Employment Type Flow Analysis

---

## 🔍 Key Insights

- Unemployed borrowers default at 3.69% versus 2.36% for 
  full-time employees — making them 57% higher risk

- Default rates peaked in 2016–2017 at 11.75%, which aligns 
  directly with the loan volume growth spike in the same period

- Home loans are the largest borrowing segment at 6,545M, 
  followed by Business loans at 6,522M

- Adults borrow the highest average loan amount at 127,901 
  while Teens borrow the least at 126,674

- Borrowers with higher credit scores request slightly lower 
  loan amounts — indicating financially responsible behavior

- High income borrowers are predominantly full-time employed 
  yet still represent a significant share of total defaults, 
  proving that income alone is not a reliable default predictor

---

## 📂 Dataset Description

The Loan Default Dataset contains information about borrowers 
who have applied for loans, along with details about their 
financial status, loan characteristics, and repayment behavior.

| Column | Type | Description |
|---|---|---|
| LoanAmount | Numeric | Total loan amount requested or approved |
| CreditScore | Numeric | Borrower creditworthiness score (300–850) |
| Age | Numeric | Age of the borrower |
| MonthsEmployed | Numeric | Months employed at current job |
| NumCreditLines | Numeric | Number of active credit lines |
| InterestRate | Numeric | Annual percentage rate charged (APR) |
| LoanTerm | Numeric | Loan repayment period in months |
| DTIRatio | Numeric | Debt-to-Income ratio of the borrower |
| Income | Numeric | Annual income of the borrower |
| Education | Categorical | Highest education level completed |
| EmploymentType | Categorical | Full-time, Part-time, Self-employed, Unemployed |
| MaritalStatus | Categorical | Single, Married, or Divorced |
| HasMortgage | Boolean | Whether borrower has an existing mortgage (Yes/No) |
| HasDependents | Boolean | Whether borrower has dependents (Yes/No) |
| LoanPurpose | Categorical | Primary reason for the loan |
| HasCoSigner | Boolean | Whether a co-signer is present (Yes/No) |
| Default | Boolean | TARGET — whether borrower defaulted (Yes/No) |
| LoanDate | Date | Date the loan was issued (DD/MM/YYYY) |

---

## ⚙️ Calculated Columns and DAX Measures Created

The following columns and measures were created inside Power BI:

*Calculated Columns:*
- Age Groups — Bucketed Age into Teen, Adults, Middle Age Adults, Senior Citizens
- Credit Score Bins — Categorized CreditScore into Low, Medium, High, Very Low
- Income Bracket — Grouped Income into High, Medium, and Low
- Year — Extracted from LoanDate for time-intelligence analysis

*DAX Measures:*
- YOY Loan Amount Change — Year-over-year percentage change in total loan amount
- YOY Default Loans Change — Year-over-year change in default loan volume
- Default Rate % — Total defaulted loans divided by total loans multiplied by 100
- Average Income by Employment Type — Average income segmented by job category
- Median Loan Amount — Median loan value by credit score category

---

## 🛠️ Tools Used

- Microsoft Power BI Desktop — Dashboard design and data visualization
- Microsoft Excel — Dataset storage and column documentation
- DAX (Data Analysis Expressions) — Custom measures and calculations
- Power Query — Data transformation and calculated columns

---

## 📸 Screenshots

### Page 1 — Loan Default and Overview


("C:\Users\ASUS\OneDrive\Desktop\UDEMY Project\Dataflow Project\Loan Default & Overview.png")



### Page 2 — Applicant Demographics and Financial Profile


![Page 2](screenshots/page2_demographics.png)



### Page 3 — Financial Risk Matrix


![Page 3](screenshots/page3_risk_matrix.png)



---

## 👁️ How To View This Project

1. Download the LoanDefault_Dashboard.pbix file from this repository
2. Download Power BI Desktop for free from microsoft.com/power-bi
3. Open Power BI Desktop
4. Click File and then Open
5. Select the downloaded .pbix file
6. Navigate through all 3 report pages using the tabs at the bottom

---

## 👤 Author

*Arpit*
Aspiring Data Analyst

LinkedIn: linkedin.com/in/yourprofile
GitHub: github.com/yourusername
Email: youremail@gmail.com

---

## 📝 Note

This project was built as part of my data analytics portfolio 
to demonstrate skills in Power BI, DAX, data modeling, and 
business insight generation using real-world financial data.
