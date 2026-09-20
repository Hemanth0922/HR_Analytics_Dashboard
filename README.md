# HR Analytics Dashboard | Power BI

An interactive Power BI dashboard that analyzes HR data for 183 employees across India and New Zealand, covering headcount, gender split, age distribution, and salary by department.



![Dashboard](dashboard.png)



## Dataset
- **File:** `hr-data.xlsx` (183 rows, 8 columns)
- **Columns:** Name, Gender, Age, Rating, Date Joined, Department, Salary, Country
- **Departments:** Procurement, Website, Finance, Sales, HR
- **Countries:** India (IND), New Zealand (NZ)

## Visuals Built

**1. Headcount by Department**
Column chart with Department on the X-axis and a `Head count` measure (count of employees) on the Y-axis.

**2. Headcount by Department and Gender**
Clustered column chart with Gender as the legend. The dataset also has an "Other" category (6 employees), which I filtered out to compare Male and Female only.

**3. Age Distribution (Histogram)**
Stacked column chart using a custom **Age bin** group (bin size 5). Conditional formatting highlights age groups with 20+ employees in a different color from smaller groups.

**4. Salary Summary by Department**
Table with three DAX measures (**Min, Max, Average Salary**), formatted to 0 decimals, plus a **Country slicer** to view each country's values separately.

## Key Insights
- Procurement (55) and Website (54) are the largest departments; HR is the smallest (8).
- The 30-34 age group is the largest, with 67 employees.
- HR has the highest average salary (~$89.6K) and Sales the lowest (~$67.9K). HR has only 8 people, so its average is less reliable.
- Overall average salary is ~$77.2K, ranging from $33.9K to $119.1K.

## Tools Used
- Power BI Desktop
- DAX (custom measures)
- Excel (data source)

## Files
- `HR-Analytics-Dashboard.pbix`: Power BI report
- `hr-data.xlsx`: source data

## Author
Hemanth
