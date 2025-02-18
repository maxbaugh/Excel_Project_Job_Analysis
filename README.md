# Data Analytics Project
Hello! check out my amazing dashboard that helps job seekers determine which data jobs offer the highest salaries.

## Intro 
The dashboard was created to help job seekers land a job and help them determine the highest salary possible.

## Excel Skills Used

- 📈**Charts**
- 🧮**Formulas and Functions**
- ✅**Data Validation**

## Data Jobs Dataset 
The 2023 data originates from [SQL Course](https://lukebarousse.com/excel). It's packed with insights on job titles, salaries, locations, and essential skills.

- 🏬**Job Titles**
- 💰**Salaries**
- 🗺️**Locations**
- 🛠️**Skills**

# Excel Dashboard

## 📈Charts

![alt text](Excel%20Project/Dashboard.png)
Use this dashboard for comparing data jobs and their salaries worldwide. Gain valuable insights into global salary trends and make informed career decisions with ease.

### Data Science Job Salaries

![[Pasted image 20250218094313.png]]

- 🧰**Excel Features** - Optimized bar chart with salary values for clarity
- 🎨**Design Choice** - Horizontal layout for better readability
- 💹**Data Organization** - Sorted salaries from largest to smallest
- 💡**Insights Gained** - Senior Engineers make more money than Analysts

![[Pasted image 20250218095429.png]]

- 🧰**Excel Features** - Excel's map chart feature plots salaries globally
- 🎨**Design Choice** - Shades of blue differentiate salary levels
- 💹**Data Representation** - Median salaries are used for each country
- 💡**Insights Gained** - Salaries across the globe are now easy to locate 

## 🧮Formulas and Functions

```
=MEDIAN(
  IF(
    (jobs[job_title_short]=A3)*
    (jobs[salary_year_avg]<>0)*
    (jobs[job_country]=country)*
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type]))),
    jobs[salary_year_avg]
  )
)
```

- 📊 **Calculates Median Salary** – Finds the median salary for a specific job title in the dataset.
- 🌍 **Filters by Country** – Includes only jobs that match the selected country.
- ⏳ **Checks Job Type** – Ensures the schedule type contains the specified keyword.
- 🚫 **Excludes Zero Salaries** – Ignores entries where the salary is missing or zero.

[Check out my work here](Excel%20Project/Project_Dashboard.xlsx)

## ✅Data Validation

![[Pasted image 20250218135647.png]]

- ✅ **Dropdown for Job Title** – Uses data validation to ensure users can only select from predefined job titles.
- 🔎 **Accurate Median Calculation** – Ensures the displayed salary updates dynamically based on the selected job.
- 📊 **Consistent Data Filtering** – Restricts salary analysis to valid job titles, preventing errors or mismatched data.

---
# Salary Analysis
![alt text](Excel%20Project/top_skills-2.png)

 I found that SQL, Excel, and Tableau are highly sought after skills. Mastering them will expand your career prospects in data analysis.

![alt text](Excel%20Project/more_skills_more_money-3.png)

This goes to show that while learning more skills can boost your earning potential, specializing in the right areas can be just as valuable.

[Check out my work here](Excel%20Project/Project_Analysis.xlsx)

# Conclusion 
Through my analysis, I learned that data job salaries vary significantly across the globe, highlighting the importance of location in career decisions. Furthermore, I discovered that SQL, Excel, and Tableau are among the most in-demand skills for Data Analysts in the U.S. Using the dataset I leveraged the power of Power Query, PivotTables, DAX, and charts. This project reinforced the value of data-driven insights in understanding job market trends and making strategic career moves.
