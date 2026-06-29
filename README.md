# Data Science Salary Dashboard

<img width="1330" height="578" alt="image" src="https://github.com/user-attachments/assets/d131104d-3e7c-4cca-b9d5-306eee5405a6" />

## Introduction

This project was created to help investigate the median salaries across various data roles and countries to make sure they are being well compensated.

The data was provided by an Excel course, which contains various columns like job titles, salaries, location, and job type.

### Skills Used
- Charts
- Formulas
- Data Validation

## Charts

<b> Bar Chart W/ Median Salary KPI Card</B>

<img width="608" height="627" alt="image" src="https://github.com/user-attachments/assets/9e41d542-0974-4ff5-acee-ecf763d2d79d" />

- Used a bar chart to show every roles median salary for clarity
- Sorted jobs in descending order, showing the highest salary first
- Created KPI card to know exactly what the median salary is, depending on the role chosen
- Gained insight on the trend that as you move up to scientist or engineer roles, the median salary goes up

<img width="619" height="639" alt="image" src="https://github.com/user-attachments/assets/2ff87210-98cc-4903-9a39-f19a11800204" />

- Plotted median salaries globally using Excel's map chart feature
- Enables a grasp of the median salary for each country
- Color-coded the map to make it clear which countries were paying the most

### Formulas 

```
=MEDIAN(
IF(
   (jobs[job_title_short]=A2)*
   (jobs[salary_year_avg]<>0)*
   (jobs[job_country]=country)*
   (ISNUMBER(SEARCH(type,jobs[job_schedule_type]))),
    jobs[salary_year_avg]
  )
)
```
<img width="224" height="212" alt="image" src="https://github.com/user-attachments/assets/bc68eba7-49e5-41e2-bc62-1d161415daf7" />

- Utilized `MEDIAN()` and `IF()` to analyze an array
- Forming this table helps us analyze each role's median salary and use it to form our chart

<img width="546" height="653" alt="image" src="https://github.com/user-attachments/assets/615bbff6-139a-468c-a983-e1baf89e48e9" />







