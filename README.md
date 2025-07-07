<h1>🔐 Apply Filters to SQL Queries</h1>


<h2>📘 Project Description</h2>
My organization is working to improve system security. As part of this effort, I investigate potential security incidents, apply system updates, and analyze login activity. This project demonstrates how I used SQL queries with filters to retrieve specific security-related data.
<br />


<h2>Language and Utility Used</h2>

- <b>SQL</b> 
  
<h2>Environments Used </h2>

- <b>Online Lab</b> (21H2)

<h2>🧪 Use Cases & SQL Queries:</h2>

<b>
<h2>1. 🕕 Retrieve After-Hours Failed Login Attempts: <br/></h2>
<b/> <p></p>
<b>There was a potential security incident that occurred after business hours (after 18:00). All after hours login attempts that failed need to be investigated.

The following code demonstrates how I created a SQL query to filter for failed login attempts that occurred after business hours.
</b>

![image alt](https://github.com/KaiFaley/-Apply-Filters-to-SQL-Queries/blob/ad9ac328b6378f1791f22a4249c5570b0fda0574/sqlimage1.png)

<b/> <p></p>
<b>The first part of the screenshot is my query, and the second part is a portion of the output. This query filters for failed login attempts that occurred after 18:00. First, I started by selecting all data from the log_in_attempts table. Then, I used a WHERE clause with an AND operator to filter my results to output only login attempts that occurred after 18:00 and were unsuccessful. The first condition is login_time > '18:00', which filters for the login attempts that occurred after 18:00. The second condition is success = FALSE, which filters for the failed login attempts. 
</b>


<b>
<h2>2. 📅 Retrieve Login Attempts on Specific Dates: <br/></h2>
<b/> <p></p>
<b>A suspicious event occurred on 2022-05-09. Any login activity that happened on 2022-05-09 or on the day before needs to be investigated.

The following code demonstrates how I created a SQL query to filter for login attempts that occurred on specific dates.

</b>

![image alt](https://github.com/KaiFaley/-Apply-Filters-to-SQL-Queries/blob/d202f66407b373dcd961b6a4ee892de8b2f66b3d/sqlimage2.png)

<b/> <p></p>
<b>The first part of the screenshot is my query, and the second part is a portion of the output. This query returns all login attempts that occurred on 2022-05-09 or 2022-05-08. First, I started by selecting all data from the log_in_attempts table. Then, I used a WHERE clause with an OR operator to filter my results to output only login attempts that occurred on either 2022-05-09 or 2022-05-08. The first condition is login_date = '2022-05-09', which filters for logins on 2022-05-09. The second condition is login_date = '2022-05-08', which filters for logins on 2022-05-08.
</b>

<b>
<h2>3. Retrieve login attempts outside of Mexico: <br/></h2>
<b/> <p></p>
<b>After investigating the organization’s data on login attempts, I believe there is an issue with the login attempts that occurred outside of Mexico. These login attempts should be investigated.

The following code demonstrates how I created a SQL query to filter for login attempts that occurred outside of Mexico. 

</b>

![image alt](https://github.com/KaiFaley/-Apply-Filters-to-SQL-Queries/blob/a071646f704bd92cd62e0903b19cd3c62a9b8109/sqlimage3.png)

<b>The first part of the screenshot is my query, and the second part is a portion of the output. This query returns all login attempts that occurred in countries other than Mexico. First, I started by selecting all data from the log_in_attempts table. Then, I used a WHERE clause with NOT to filter for countries other than Mexico. I used LIKE with MEX% as the pattern to match because the dataset represents Mexico as MEX and MEXICO. The percentage sign (%) represents any number of unspecified characters when used with LIKE. 
</b>

<b>
<h2></h2>4. Retrieve employees in Marketing: <br/></h2>
<b/> <p></p>
<b>My team wants to update the computers for certain employees in the Marketing department. To do this, I have to get information on which employee machines to update.

The following code demonstrates how I created a SQL query to filter for employee machines from employees in the Marketing department in the East building.

</b>

![image alt](https://github.com/KaiFaley/-Apply-Filters-to-SQL-Queries/blob/a071646f704bd92cd62e0903b19cd3c62a9b8109/sqlimage4.png)

<b>The first part of the screenshot is my query, and the second part is a portion of the output. This query returns all employees in the Marketing department in the East building. First, I started by selecting all data from the employees table. Then, I used a WHERE clause with AND to filter for employees who work in the Marketing department and in the East building. I used LIKE with East% as the pattern to match because the data in the office column represents the East building with the specific office number. The first condition is the department = 'Marketing' portion, which filters for employees in the Marketing department. The second condition is the office LIKE 'East%' portion, which filters for employees in the East building. 
</b>

<b>
<h2></h2>5. Retrieve employees in Finance or Sales: <br/></h2>
<b/> <p></p>
<b>The machines for employees in the Finance and Sales departments also need to be updated. Since a different security update is needed, I have to get information on employees only from these two departments.

The following code demonstrates how I created a SQL query to filter for employee machines from employees in the Finance or Sales departments.

</b>

![image alt](https://github.com/KaiFaley/-Apply-Filters-to-SQL-Queries/blob/a071646f704bd92cd62e0903b19cd3c62a9b8109/sqlimage5.png)

<b>The first part of the screenshot is my query, and the second part is a portion of the output. This query returns all employees in the Finance and Sales departments. First, I started by selecting all data from the employees table. Then, I used a WHERE clause with OR to filter for employees who are in the Finance and Sales departments. I used the OR operator instead of AND because I want all employees who are in either department. The first condition is department = 'Finance', which filters for employees from the Finance department. The second condition is department = 'Sales', which filters for employees from the Sales. 
</b>

<b>
<h2></h2>6. Retrieve all employees not in IT: <br/></h2>
<b/> <p></p>
<b>My team needs to make one more security update on employees who are not in the Information Technology department. To make the update, I first have to get information on these employees.

The following demonstrates how I created a SQL query to filter for employee machines from employees not in the  Information Technology department.

</b>

![image alt](https://github.com/KaiFaley/-Apply-Filters-to-SQL-Queries/blob/a071646f704bd92cd62e0903b19cd3c62a9b8109/sqlimage6.png)

<b>The first part of the screenshot is my query, and the second part is a portion of the output. The query returns all employees not in the Information Technology department. First, I started by selecting all data from the employees table. Then, I used a WHERE clause with NOT to filter for employees not in this department.
</b>


<h2>🧪 Summary:</h2>
</>
<b>I applied filters to SQL queries to get specific information on login attempts and employee machines. I used two different tables, log_in_attempts and employees. I used the AND, OR, and NOT operators to filter for the specific information needed for each task. I also used LIKE and the percentage sign (%) wildcard to filter for patterns.
</b>

