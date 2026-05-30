# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: BHUVANESH K
* **Register Number**: 212224230037
* **Date of Submission**: 30-05-2026

---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow (Student Explanation)

1.First, a security group named DB Security Group was created to allow the web server to connect to the database using port 3306 (MySQL).
2.A DB Subnet Group was created with subnets from two Availability Zones to allow the database to run in a Multi-AZ environment for high availability.
3.A MySQL RDS instance named lab-db was created with the database name lab, username main, and password lab-password.
4.The database was associated with the DB Security Group and the Lab VPC so that the web server can securely connect to the database.
5.The web application running on the EC2 server was opened using its IP address, and the RDS endpoint, database name, username, and password were entered to interact with the database.

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server


<img width="1919" height="1054" alt="Screenshot 2026-05-15 205807" src="https://github.com/user-attachments/assets/e809ab20-60ce-4d8e-933a-8c255eb9d91a" />


---

### Screenshot 2: Database Service Running

(Insert Screenshot Here)

<img width="1919" height="1057" alt="Screenshot 2026-05-15 211701" src="https://github.com/user-attachments/assets/67bc8e9d-0f73-4740-a80a-dd6e2f5ab715" />

---

### Screenshot 3: Sample Database and Table

<img width="1919" height="1101" alt="Screenshot 2026-05-15 212351" src="https://github.com/user-attachments/assets/f3965d30-2e9f-4ed4-8055-bc59a3a5f09d" />


---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst
