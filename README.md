📌 # Project Objective

The objective of this project is to deploy a Java-based application on an Amazon EC2 instance and connect it with an AWS RDS MySQL database. The application performs basic CRUD operations, while MySQL Workbench is used for remote database administration. This project demonstrates a secure and scalable cloud-based application architecture.

📌 Project Overview

A Java application is hosted on an EC2 instance (Linux/Windows) acting as the application layer.

The application connects to an AWS RDS MySQL database using a JDBC connection string.

Developers use MySQL Workbench locally to manage schemas, run queries, and monitor the database.

AWS Security Groups control secure access between EC2, RDS, and MySQL Workbench.

The architecture represents a real-world cloud deployment where compute and database layers are separated.

📌 Architecture Workflow

Step-by-step flow:

1) Client Request – End users access the Java application running on EC2.

2) Application Layer (EC2) – Java code processes requests and communicates with the database.

3) Database Layer (RDS MySQL) – Executes Insert, Select, Update, and Delete operations.

4) Database Management – MySQL Workbench connects securely to RDS for administration and monitoring.

5) Data Exchange – Data flows between EC2 ↔ RDS and RDS ↔ MySQL Workbench.
   
<img width="1536" height="1024" alt="Architecture Diagram" src="https://github.com/user-attachments/assets/3179b782-0336-437c-81e4-7e471bfd9cb1" />


📌 Key Advantages

1)  Scalability – EC2 and RDS can be scaled independently based on application load.
2) Loose Coupling – Application and database are separated, improving system stability.
3) High Availability – RDS supports automated backups, snapshots, and Multi-AZ deployments.
4) Security – Access is restricted using AWS Security Groups and database credentials.
5) Operational Simplicity – MySQL Workbench enables easy database management without EC2 access.
6) Cost Efficiency – Pay-as-you-go pricing with flexible scaling options.
