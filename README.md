# 📊 HR Analytics

This project was completed as part of my Data Analysis internship at **Syntecxhub**.

The main goal of this project was to analyze employee information and understand patterns related to **employee attrition, salary, experience, job roles, overtime and job satisfaction**.

I worked with the dataset using Python for data cleaning and analysis, and then used Power BI to create an interactive HR Analytics dashboard.

---

## 📌 Project Objective

The objective of this project was to:

- Understand the overall employee workforce
- Analyze employee attrition
- Compare attrition across departments and job roles
- Analyze salary and work experience
- Identify factors associated with employee attrition
- Understand the relationship between overtime and attrition
- Analyze employee job satisfaction
- Create an interactive dashboard for HR-related insights

---

## 📂 Dataset

The original dataset contains:

- **1,480 rows**
- **38 columns**

The dataset contains employee-related information such as:

- Age
- Gender
- Department
- Job Role
- Monthly Income
- Total Working Years
- Years at Company
- Years in Current Role
- Years Since Last Promotion
- Years With Current Manager
- Overtime
- Job Satisfaction
- Environment Satisfaction
- Work-Life Balance
- Business Travel
- Marital Status
- Education
- Performance Rating
- Attrition

The original dataset is included in this repository as:

`HR_Analytics.csv`

---

## 🧹 Data Cleaning

Before starting the analysis, I checked the dataset for missing values and duplicate records.

### Initial checks

- **7 duplicate rows** were found.
- **57 missing values** were found in `YearsWithCurrManager`.
- `EmployeeCount` and `StandardHours` had constant values and were not useful for analysis.

### Cleaning steps

I:

1. Created a separate copy of the original dataset for cleaning.
2. Removed duplicate records.
3. Filled the missing `YearsWithCurrManager` values using the median.
4. Removed constant columns.
5. Verified that the cleaned dataset had no missing values or duplicate rows.

After cleaning, the dataset contained:

- **1,473 rows**
- **36 columns**

The cleaned dataset is included as:

`HR_Analytics_Cleaned.csv`

---

## 🔎 Analysis Performed

### Employee Attrition

The cleaned dataset contains:

- **1,236 employees who stayed**
- **237 employees who left**
- **16.09% overall attrition rate**
- **83.91% retention rate**

### Department Analysis

I compared employee attrition across:

- Human Resources
- Research & Development
- Sales

I also calculated the attrition rate for each department.

### Job Role Analysis

I compared attrition across different job roles and calculated the attrition rate for each role.

The highest attrition rate was observed for:

**Sales Representative — 39.29%**

### Overtime Analysis

I compared attrition between employees who worked overtime and those who did not.

The attrition rate was:

- **No Overtime — 10.41%**
- **Overtime — 30.53%**

### Salary and Experience

I analyzed:

- Average monthly salary
- Average work experience
- Salary by department
- Relationship between salary and total working years

### Job Satisfaction

The average job satisfaction score was:

**2.73**

I also compared average job satisfaction across departments.

---

## 🔗 Correlation Analysis

I created an attrition flag where:

- `No = 0`
- `Yes = 1`

Then I calculated correlations between numerical employee attributes and attrition.

Some of the stronger negative correlations were:

| Factor | Correlation |
|---|---:|
| Total Working Years | -0.171 |
| Job Level | -0.169 |
| Years in Current Role | -0.160 |
| Monthly Income | -0.159 |
| Age | -0.159 |
| Years With Current Manager | -0.158 |
| Stock Option Level | -0.137 |
| Years At Company | -0.134 |

Distance From Home had a positive correlation of approximately **0.078**.

These values show associations in the dataset and should not be interpreted as direct causes of employee attrition.

---

## 📊 Power BI Dashboard

After completing the Python analysis, I created an interactive **HR Analytics Dashboard** in Power BI.

### KPI Cards

The dashboard includes:

- 👥 Total Employees — **1,473**
- 🚪 Employees Left — **237**
- 📉 Attrition Rate — **16.09%**
- 💰 Average Monthly Salary — **6,500.23**
- 💼 Average Experience — **11.28 years**
- 😊 Average Job Satisfaction — **2.73**

### Dashboard Visuals

The dashboard includes:

- Employee Headcount by Department
- Employee Attrition Distribution
- Attrition Rate by Job Role
- Average Salary by Department
- Attrition by Overtime
- Attrition by Department
- Salary vs Experience
- Average Job Satisfaction by Department
- Factors Associated with Attrition

### Interactive Filters

The dashboard also includes filters for:

- 🏢 Department
- 💼 Job Role
- 👤 Gender
- ⏱️ OverTime
- 💍 Marital Status

These filters allow different parts of the dashboard to be explored interactively.

---

## 🛠️ Tools Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Jupyter Notebook**
- **Power BI**
- **GitHub**

---

## 📁 Project Files

```text
Syntecxhub_HR_Analytics/
│
├──01_HR Analytics.ipynb
├──02_HR Analytics.csv
├──03_HR Analytics Cleaned.csv
├──04_HR Analytics Dashboard.pbix
└── README.md
```

## Thank You

Thank you to **Syntecxhub** for providing this internship opportunity and giving me the chance to work on practical data analysis projects.

This project helped me gain hands-on experience with Python, data analysis and Power BI, and I look forward to applying these skills to more real-world projects.
