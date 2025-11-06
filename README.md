Description:
This project demonstrates the process of cleaning, transforming, and analyzing expense data using Power BI and Power Query. The goal was to automate data corrections, apply custom transformations, and generate insightful reports for business decision-making.

Key Steps and Features:

Data Cleansing and Correction:
Corrected spelling and punctuation errors in the Expense Type column.
Standardized project names to ensure uniformity across the dataset.

Custom Column Creation:
Added a custom column to handle missing currency values based on the amount, applying a logical formula:
If the currency is missing and the amount is greater than or equal to 1000, the currency is set to "INR."
If the currency is missing and the amount is less than 1000, the currency is set to "USD."
Otherwise, the existing currency value remains unchanged.

Currency Conversion to INR:
Implemented logic to convert the "Amount" column into INR based on the currency:
Used predefined exchange rates for USD and EUR to INR conversion.
Rows with missing or INR values remain unchanged.

Financial Insights and Measures:
Created a Measure to calculate the sum of reimbursed amounts in INR across all entries.
Created another Measure to calculate the total reimbursed amount for a specific project, "Project_B."

Declined Requests Tracking:
Developed a measure to count the number of declined requests based on certain conditions, helping to track and analyze project-related declines.

Interactive Visuals and Reports:
Built slicers for Project and Employee, allowing users to filter data dynamically.
Created a Bar Chart to display the reimbursement amounts per employee.
Developed a Pie Chart to visualize the reimbursement amounts across different projects.
