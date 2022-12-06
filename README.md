# sql-datamodeling-engineering-analysis
![data enginering](https://user-images.githubusercontent.com/109861849/205740610-cff1a40c-34c8-4b6d-a156-a93e5ada2bb5.png)
# Data Modeling, Data Engineering, Data Analysis

## Notes about the Project
This project is divided into three parts: data modeling, data engineering, and data analysis. Source files are included in ‘data’ folder

## Objective of the Analysis 
Conduct a research project about people whom the company employed during the 1980s and 1990s using six CSV files.
### Data Modeling
Entity Relationship Diagram of the tables sketched using QuickDBD.
![QuickDBD-Employees](https://user-images.githubusercontent.com/109861849/205788540-94c71c66-b73d-4ca1-a26d-fb1ffbdbd7b7.png)

### Data Engineering
1.	ER diagram used to create table schema in Postgresql for each of the six CSV files. Care was taken to:
○	to specify the data types, primary keys, foreign keys, and other constraints.
○	For the primary keys, verification was made for each column if it is unique. Otherwise, a composite key was created containing two primary keys to uniquely identify a row.
○	Tables were imported in the correct order to handle the foreign keys.
2.	Import each CSV file into its corresponding SQL table.
Care was taken to import the data in the same order as the corresponding tables got created. And, header orders were accounted for during importing.
(Get sql file of tables schema in employees folder)
### Data Analysis
The following exploratory analysis were conducted on the imported data set:
1.	List the employee number, last name, first name, sex, and salary of each employee.
2.	List the first name, last name, and hire date for the employees who were hired in 1986.
3.	List the manager of each department along with their department number, department name, employee number, last name, and first name.
4.	List the department number for each employee along with that employee’s employee number, last name, first name, and department name.
5.	List first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B.
6.	List each employee in the Sales department, including their employee number, last name, and first name.
7.	List each employee in the Sales and Development departments, including their employee number, last name, first name, and department name.
8.	List the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name).
(Get SQL queries code in employees folder)
