# HR Analytics Dashboard 2023

## Overview
This Power BI report provides an in-depth analysis of the HR metrics at an organization, focusing on employee attrition, departmental performance, job satisfaction, and educational breakdowns. The report is designed to help HR professionals monitor employee retention, job satisfaction, and identify trends in attrition across various demographics such as age, gender, and education level.

## Key Features
- **Total Employees**: Displays the total number of employees at the organization.
- **Attrition Count and Rate**: Provides insights into employee attrition, including the total number of employees who left the company and the attrition rate as a percentage of the workforce.
- **Attrition by Department**: A pie chart showcasing attrition rates broken down by department.
- **Job Satisfaction Ratings**: A Matrix with heatmap that reveals job satisfaction ratings for various roles, allowing stakeholders to identify areas where employees may be unhappy.
- **Attrition by Age and Gender**: Stacked column charts and donut charts highlighting employee attrition based on age group and gender, offering a deeper demographic view.
- **Education and Attrition**: A stacked bar chart that shows the attrition rates across different education levels, revealing the impact of education on employee retention.

## Data Source
- **HR Data.csv**: This dataset contains records on employee attrition, department, age group, gender, education level, and job satisfaction ratings. Key fields include `Employee_ID`, `Attrition`, `Department`, `Age`, `Gender`, `Education`, and `Job_Satisfaction`.

## Visualizations

### 1. **Department Wise Attrition**
- **Type**: Pie Chart
- **Purpose**: Displays the percentage of employees leaving from each department.
- **Insight**: The highest attrition is seen in the R&D department (56.12%), with the HR department having the least attrition (5.06%).

### 2. **Employee Age and Gender Breakdown**
- **Type**: Stacked Column Chart
- **Purpose**: This chart shows the distribution of employees by age group and gender, along with a breakdown of attrition rates for each category.
- **Insight**: Attrition is highest among employees in the 25-34 age group, with 112 employees leaving (61.61%).

### 3. **Job Satisfaction Ratings**
- **Type**: Matrix
- **Purpose**: Provides a visual of job satisfaction across various roles on a scale from 1 to 4.
- **Insight**: Research Scientists and Sales Executives show the highest job satisfaction, while Human Resources has lower satisfaction ratings.

### 4. **Attrition by Education**
- **Type**: Stacked Bar Chart
- **Purpose**: Compares attrition rates based on employees' education levels.
- **Insight**: Employees with a Bachelor's degree have the highest attrition rate (99 employees), while those with Doctoral degrees show the least attrition (5 employees).

### 5. **Attrition Rate by Gender for Different Age Groups**
- **Type**: Donut Chart
- **Purpose**: Displays the attrition rate segmented by gender for each age group.
- **Insight**: Males in the 25-34 age group show the highest attrition rate (61.61%).

## KPIs
- **Total Employees**: 1,470
- **Attrition Count**: 237
- **Attrition Rate**: 16.12%
- **Active Employees**: 1,233
- **Average Employee Age**: 37 years

These KPIs provide a quick summary of the organization’s workforce status and employee retention.

## DAX Formulas

Here are some of the DAX formulas used in the report to compute key metrics:

- **Attrition Count**:
  ```DAX
  Attrition count = COUNTX(FILTER('HR Data','HR Data'[Attrition] = "Yes"),1) 
- **Attrition Rate**:
  ```DAX
  Attrition rate = SUM('HR Data'[Attrition Count])/SUM('HR Data'[Employee Count])
## Insights & Learnings
- Attrition is most common among employees aged 25-34, particularly in the R&D department.
- Sales Executives have the highest job satisfaction, whereas the Human Resources department shows signs of dissatisfaction.
- Employees with Bachelor’s degrees experience the highest attrition, while those with Doctoral degrees have a much lower turnover.
  
## Screenshots

![image](https://github.com/user-attachments/assets/06c66c94-6061-420e-b45a-e2e961f21351)

![image](https://github.com/user-attachments/assets/267e09a2-c97e-4db1-9107-5ee3ed4c15b9)

![image](https://github.com/user-attachments/assets/a9f8f800-47f0-4991-b80b-64f5159b3ee5)

![image](https://github.com/user-attachments/assets/af52d57f-0a7a-414a-816e-d2399e8dc3de)

![image](https://github.com/user-attachments/assets/37c9bf9f-b4b5-4f9c-8a43-4b373f219c92)

## Tools And Technologies
- **Power BI**: Used for data visualization and analysis.
- **Excel/CSV**: Data source for HR metrics.
  
## Conclusion
The HR Analytics Dashboard 2023 provides a holistic view of employee retention, attrition, and satisfaction within the organization. Through detailed visualizations and metrics, the dashboard highlights key trends that can guide HR departments in improving employee engagement and reducing turnover.

Key findings indicate that the R&D department faces the highest attrition rates, particularly among employees in the 25-34 age group, a demographic that could benefit from targeted retention strategies. Additionally, the analysis reveals that employees with Bachelor's degrees experience the highest turnover, suggesting the need for more career development opportunities for this group.

On the positive side, Sales Executives and Research Scientists show high job satisfaction, underscoring the importance of maintaining a focus on job satisfaction across other roles, such as those in Human Resources, where lower satisfaction rates were observed.

By leveraging the actionable insights provided in this report, HR leaders can implement strategic initiatives to address the identified pain points—ultimately improving employee satisfaction, lowering attrition rates, and fostering a more engaged and stable workforce.














