Project Overview
The DVWA is an intentionally vulnerable web application designed for security professionals to practice techniques used in penetration testing. The focus of this report is on solving SQL Injection labs, demonstrating how attackers can manipulate queries to extract sensitive information from the database.

Objectives
Install DVWA using Docker.
Solve SQL Injection labs at Low, Medium, and High security levels.
Demonstrate successful SQL injections and analyze the results.
Highlight differences in SQL injection protection at various security levels.
Repository Contents
Report.pdf: The detailed report explaining the process of exploiting SQL Injection vulnerabilities at different security levels.
SQL_Injection_Low.md: Step-by-step execution of the SQL Injection attack at Low security level.
SQL_Injection_Medium.md: Step-by-step execution of the SQL Injection attack at Medium security level.
SQL_Injection_High.md: Explanation and testing of SQL Injection on High security level, highlighting the defenses in place.
Screenshots: A folder containing screenshots of the exploitation process at each security level.
Prerequisites
Docker installed on your system.

sudo apt install docker.io

Basic knowledge of SQL Injection and web vulnerabilities.
Tools like Burp Suite to intercept and modify HTTP requests.

Installation Instructions
Clone the Repository:
git clone https://github.com/eystsen/pentestlab.git 

cd pentestlab

Accessing to the DVWA Web Page 

 ./pentestlab.sh start dvwa

Access DVWA: Open your web browser and navigate to http://localhost:80. Login to DVWA with the default credentials:

Username: admin

Password: password

Configure DVWA:

Go to the DVWA setup page and click "Create / Reset Database."
Set the DVWA security level to Low, Medium, and High for the respective SQL Injection tests.
Usage
Follow the steps outlined in the SQL_Injection_Low.md, SQL_Injection_Medium.md, and SQL_Injection_High.md files to replicate the SQL injection attacks.
Use Burp Suite to intercept and modify requests as needed.
Analyze the differences in security mechanisms across the three levels.
Results and Observations
SQL injection vulnerabilities were successfully exploited at Low and Medium security levels.
High security level demonstrated increased protection against SQL injection, requiring more advanced techniques to bypass.
Conclusion
This project highlights the importance of proper input validation and secure coding practices to mitigate SQL injection vulnerabilities. By progressing through different security levels, the report provides insights into how defenses can evolve to reduce the risk of SQL injection attacks.
