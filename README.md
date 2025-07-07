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
1. 🕕 Retrieve After-Hours Failed Login Attempts: <br/>
<b/> <p></p>
<b>There was a potential security incident that occurred after business hours (after 18:00). All after hours login attempts that failed need to be investigated.

The following code demonstrates how I created a SQL query to filter for failed login attempts that occurred after business hours.
</b>

![image alt](https://github.com/KaiFaley/-Apply-Filters-to-SQL-Queries/blob/ad9ac328b6378f1791f22a4249c5570b0fda0574/sqlimage1.png)

<b/> <p></p>
<b>The first part of the screenshot is my query, and the second part is a portion of the output. This query filters for failed login attempts that occurred after 18:00. First, I started by selecting all data from the log_in_attempts table. Then, I used a WHERE clause with an AND operator to filter my results to output only login attempts that occurred after 18:00 and were unsuccessful. The first condition is login_time > '18:00', which filters for the login attempts that occurred after 18:00. The second condition is success = FALSE, which filters for the failed login attempts. 
</b>


<b>
2. 📅 Retrieve Login Attempts on Specific Dates: <br/>
<b/> <p></p>
<b>A suspicious event occurred on 2022-05-09. Any login activity that happened on 2022-05-09 or on the day before needs to be investigated.

The following code demonstrates how I created a SQL query to filter for login attempts that occurred on specific dates.

</b>

![image alt](https://github.com/KaiFaley/-Apply-Filters-to-SQL-Queries/blob/ad9ac328b6378f1791f22a4249c5570b0fda0574/sqlimage1.png)



<h2>🧪 Use Cases & SQL Queries:</h2>

<b>
1. 🕕 Retrieve After-Hours Failed Login Attempts: <br/>
<b/> <p></p>
<b>There was a potential security incident that occurred after business hours (after 18:00). All after hours login attempts that failed need to be investigated.

The following code demonstrates how I created a SQL query to filter for failed login attempts that occurred after business hours.
</b>

![image alt](https://github.com/KaiFaley/-Apply-Filters-to-SQL-Queries/blob/ad9ac328b6378f1791f22a4249c5570b0fda0574/sqlimage1.png)



<h2>🧪 Use Cases & SQL Queries:</h2>

<b>
1. 🕕 Retrieve After-Hours Failed Login Attempts: <br/>
<b/> <p></p>
<b>There was a potential security incident that occurred after business hours (after 18:00). All after hours login attempts that failed need to be investigated.

The following code demonstrates how I created a SQL query to filter for failed login attempts that occurred after business hours.
</b>

![image alt](https://github.com/KaiFaley/-Apply-Filters-to-SQL-Queries/blob/ad9ac328b6378f1791f22a4249c5570b0fda0574/sqlimage1.png)
