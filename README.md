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

- Unemployed borrowers default at a rate of 3.49% versus 2.36% for 
  full-time employees — making employment status a major risk indicator.

- Default rates saw a historical peak in the year 2016 at exactly 11.75%.

- Home loans are the largest borrowing segment by volume at $6.54B, 
  followed closely by Business loans at $6.52B.

- Adult age groups borrow the highest average loan amount at $127,901, 
  while Teens borrow the least at $126,674.

- Borrowers with "High" credit scores have a lower median loan amount 
  ($127,149) compared to those with "Low" scores ($128,397) — indicating 
  more conservative borrowing behavior among high-credit individuals.


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

<img width="1656" height="952" alt="Loan Default   Overview" src="https://github.com/user-attachments/assets/1db61a31-8802-4985-9e02-5612ffb27c52" />





### Page 2 — Applicant Demographics and Financial Profile


<img width="1659" height="958" alt="Application Demographics   Financial Profile" src="https://github.com/user-attachments/assets/b6ccbe2c-ac39-49b7-af1b-7656949ea71b" />




### Page 3 — Financial Risk Matrix

<img width="1657" height="958" alt="Financial Risk Matrix" src="https://github.com/user-attachments/assets/18e4de99-ba65-49be-9904-c198716c7fbb" />




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

LinkedIn: www.linkedin.com/in/
arpit-amale-89796a27b

GitHub: https://github.com/ArpitAmale
Email: arpitamale100@gmail.com

---

## 📝 Note

This project was built as part of my data analytics portfolio 
to demonstrate skills in Power BI, DAX, data modeling, and 
business insight generation using real-world financial data.
