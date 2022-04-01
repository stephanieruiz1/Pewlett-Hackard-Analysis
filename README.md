# Pewlett-Hackard-Analysis
## The Purpose
Pewlett-Hackard is a large company boasting several thousand employees and it’s been around for long time. As baby boomers begin to retire at a rapid rate Pewlett-Hackard is looking toward the future in two ways. It’s starting to think about which positions will need to be filled in the near future.
Bobby is an up-and-coming HR Analyst whose task is to perform employee research and Bobby’s manager has given us a job to determine the number of retiring employees per title, and to identify employees who are eligible to participate in a mentorship program. The Task is to help Bobby build an employee database with SQL by applying data modelling, engineering and analysis.
## Results
### The table of retiriment employees
![retirement_titles](retirement_titles.png)

1) This table shows an aprox of 133776 employees.

2) The problem with this table is that some empoyees are showing 2 times because they change positions over the years
### Unique Titles
![unique_titles](unique_titles.png)

3) On this table, we use Dictinct to remove duplicate rows
 
4) The table shows the exact 72458 people that are going to retire with no duplicates
### Retiring titles
![retiring_titles](retiring_titles.png)

5) this table shows how many employess are based on their titles
### Mentorship program
![mentorship_eligibility](mentorship_eligibility.png)

1) we can see that 1549 employees are eligible for this program based on the date of birth between 01/01/65 to 12/31/65.

2) That seems to low to be able to train 72458 new employees in 4 years.

3) we use distinct (no duplicates) and joined 3 tables (department_employees,titles and employees)

4) we exclude those employees that have already left the company by filtering on to_date to keep only those dates that are equal to '9999-01-01'.
## SUMMARY
#### How many roles will need to be filled as the "silver tsunami" begins to make an impact?
The employees expected to retire are a total of 72,458 at Pewlett Hackard. 
#### Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
### This table shows how many people participate in a mentorship program and their titles
![mentor_count](mentor_count.png)

Employees who are eligible to participate in a mentorship program  are 1549 from the year of 1965. That means that each member needs to train around 46-47 people in 4 year, 11-12 per year and 1 per month. which is impossible. I would say that maximun of new employees to train is 1-2 people per year to have a good quality of new employees. 
For that reason I will recommend the mentorship program to be extended a few years between 1964-1965.After that we see that 19,905 employees will be able to train 72,458 new employees in 4 years. That is a better option because it will be 4 traines for each employee in 4 years.
### This table is mentorship extended between 1964-1965
![mentor_count1964](mentor_count1964.png)

