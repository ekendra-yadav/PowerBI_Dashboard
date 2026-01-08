# HR Analytics Dashboard: Employee Attrition & Retention

## 📌 Project Overview
This project focuses on identifying the root causes of employee attrition through data-driven insights. Using a dataset of over 1,400 employees, I built an end-to-end Power BI solution that automates data cleaning and visualizes key performance indicators (KPIs) to help HR departments reduce turnover.

---

## 🛠️ Data Cleaning & Transformation (The "ETL" Process)
*As I am seeking roles in Data Cleaning, this section highlights my technical approach to messy data:*

1.  **Data Profiling:** Used Power Query to identify null values and outliers in columns like `MonthlyIncome` and `YearsAtCompany`.
2.  **Data Standardization:** Standardized the `Attrition` column into binary formats for easier DAX calculation.
3.  **Feature Engineering:**
    * **Age Bucketing:** Created groups (18-25, 26-35, 36-45, 46-55, 55+) using **Conditional Columns**.
    * **Salary Slabs:** Categorized income into segments to identify if low pay is a driver for leaving.
4.  **Date Logic:** Ensured all tenure-related columns were formatted as whole numbers for accurate averaging.



---

## 📊 Dashboard Features & DAX Measures
The dashboard is designed for high-level management and deep-dive departmental analysis.

### **Key Measures Created:**
* **Total Employees:** `COUNT(HR_Data[EmployeeID])`
* **Attrition Rate:** `DIVIDE(CALCULATE(COUNT(HR_Data[Attrition]), HR_Data[Attrition]="Yes"), [Total Employees], 0)`
* **Average Tenure:** `AVERAGE(HR_Data[YearsAtCompany])`

### **Visualizations Included:**
* **Attrition by Education:** Bar chart showing which academic backgrounds stay longest.
* **Job Satisfaction Heatmap:** Matrix visual correlating job roles with satisfaction scores.
* **Demographic Breakdown:** Donut charts for gender and marital status impact on retention.



---

## 💡 Top Business Insights
* **The "Early Exit" Trend:** Employees are at the highest risk of leaving during their **first 2 years**. Better onboarding is recommended.
* **Income Impact:** Attrition is significantly higher for employees earning less than **$5,000/month**.
* **Role Specifics:** **Sales Representatives** have the highest turnover rate compared to Research Scientists.

---

## ⚙️ How to View This Project
1.  **Download** the `.pbit` (Power BI Template) file from this repo.
2.  **Open** it in Power BI Desktop.
3.  The dashboard structure and cleaning steps will be visible under the **"Transform Data"** settings.

---

## 📞 Contact
If you are looking for a Data Analyst with strong visualization and cleaning skills, feel free to reach out!
* **LinkedIn:** https://www.linkedin.com/in/ekendra-yadav-2aa76b256/
