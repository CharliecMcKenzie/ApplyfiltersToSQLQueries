# Apply filters to SQL queries

## Project description
My organization is enhancing its system security, and my role is to ensure its safety by investigating potential security issues and updating employee computers as needed. Here are some examples of how I used SQL filters for security-related tasks.

## Project walk-through:

### Retrieve Failed Login Attempts After Hours
We experienced a potential security incident after business hours (after 18:00). All failed login attempts during this period need to be examined.

The following SQL query demonstrates how to filter for failed login attempts that occurred after business hours.
<p align="center">
<img src="https://i.imgur.com/ZACe7Pk.png" height="80%" width="80%" alt="SQLfilters"/>

This query selects data from the 'log_in_attempts' table, filtering for login attempts that occurred after 18:00 and were unsuccessful.

### Retrieve Login Attempts on Specific Dates
A suspicious event occurred on 2022-05-09. We need to investigate login activities on 2022-05-09 and the preceding day.

The following SQL query demonstrates how to filter for login attempts on specific dates.
<p align="center">
<img src="https://i.imgur.com/zEczem3.png" height="80%" width="80%" alt="SQLfilters"/>

This query selects data from the 'log_in_attempts' table, filtering for login attempts on either 2022-05-09 or 2022-05-08.
  
### Retrieve Login Attempts Outside of Mexico

There is a concern with login attempts originating outside of Mexico, and these need to be investigated.

The following SQL query demonstrates how to filter for login attempts outside of Mexico.
<p align="center">
<img src="https://i.imgur.com/1mlOpBU.png" height="80%" width="80%" alt="SQLfilters"/>

This query selects data from the log_in_attempts table, filtering for login attempts that did not originate from Mexico.

### Retrieve Employees in Marketing

To update the computers for Marketing department employees in the East building, I need to identify the relevant machines.

The following SQL query demonstrates how to filter for Marketing employees in the East building.
<p align="center">
<img src="https://i.imgur.com/5c9Av75.png" height="80%" width="80%" alt="SQLfilters"/>

This query selects data from the employees table, filtering for employees in the Marketing department and the East building.

### Retrieve Employees in Finance or Sales

Different security updates are required for employees in the Finance and Sales departments. I need to identify these employees.

The following SQL query demonstrates how to filter for employees in Finance or Sales.
<p align="center">
<img src="https://i.imgur.com/FxZd4Eh.png" height="80%" width="80%" alt="SQLfilters"/>

This query selects data from the employees table, filtering for employees in either the Finance or Sales departments.

### Retrieve All Employees Not in IT

For a final security update, I need to identify employees who are not part of the Information Technology department.

The following SQL query demonstrates how to filter for employees not in IT.
<p align="center">
<img src="https://i.imgur.com/eYDtriz.png" height="80%" width="80%" alt="SQLfilters"/>

This query selects data from the employees table, filtering for employees not in the IT department.

## Summary

I utilized SQL filters to extract specific information on login attempts and employee machines, employing the log_in_attempts and employees tables. The filtering was achieved using the AND, OR, and NOT operators, as well as the LIKE operator with the % wildcard to match patterns.
