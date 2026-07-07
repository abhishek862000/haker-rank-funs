# haker-rank-funs
7-7-2026
manhatten distance <img width="399" height="762" alt="image" src="https://github.com/user-attachments/assets/924ec85e-0465-4062-addc-0386084846ed" />
 solution select
-- the abs is used to find the absolute value
round(ABS(min(LAT_N )-max(LAT_N))+ 
ABS(min(LONG_W)-max(LONG_W)),4)
 from  STATION ;

3-7-2026
Summary of the "Top Earners" ProblemThe Core Objective
You need to write an SQL query to find the absolute highest total earnings among all employees in the company, and then count exactly how many employees made that maximum amount.  Key DefinitionsTotal Earnings: Calculated by multiplying an employee's months worked by their monthly salary.  Maximum Total Earnings: The single highest earnings value found across the entire Employee table.  The Employee Table SchemaThe data is stored in a table named Employee with the following columns:employee_id (Integer): The employee's unique ID number.  name (String): The employee's name.  months (Integer): The total number of months they have worked for the company.  salary (Integer): The employee's monthly salary.  Expected OutputYour query must print exactly two integer values separated by a single space:The maximum total earnings value.  The total count of employees who achieved that specific maximum total earnings.  (For example, if the highest earnings calculated is 69952 and only 1 employee earned that amount, the expected output is simply 69952 1.)  

solutiion

SELECT months*salary as earnings,count(*) 
from Employee
GROUP BY earnings
ORDER BY earnings DESC
LIMIT 1;<img width="693" height="697" alt="image" src="https://github.com/user-attachments/assets/dcbe5cd7-cb2d-4ed2-9ddd-dedcf2b6d6ca" />


Agragate 1 st qustions <img width="365" height="300" alt="image" src="https://github.com/user-attachments/assets/53bf9faa-ed1d-4057-9929-a716f6cd701e" />

Query a count of the number of cities in CITY having a Population larger than 100000

 answer code 
SELECT count(ID) from CITY 
District
where population>100000;

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/824a9ac6-a887-4e55-b6b6-579d8cf2a0ee" />

Q2 , Query the total population of all cities in CITY where District is California.<img width="365" height="300" alt="1449729804-f21d187d0f-CITY" src="https://github.com/user-attachments/assets/83dc220c-985d-4a5f-b79d-a38169cb4fea" />

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/576620ca-57b0-4473-88ca-ed89a3c73fd8" />

