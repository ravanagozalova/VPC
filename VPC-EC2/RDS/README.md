Intro to RDS
What is RDS: managed relational database service
PaaS offering making it easier to scale and setup databases
Types of database engines that RDS supports
Commercial engines: Oracle, Microsoft SQL Server
Open Source engines: MariaDB, Postgres, MySQL
Cloud native engine: Aurora (postgres / mysql compatible)
Benefits
RDS aims to lower TCO (total cost of owners)
Self hosted vs RDS
IaaS --> creating everything from scratch
PaaS --> Create database, load data and tune queries
Configurations of RDS
DB engine
License model
DB Engine version
Instance class
Multi AZ Deployment
Storage type and size
Backups
Monitoring and maintenance
Does NOT allow shell access to the database instance
Terminology
Database instance: isolated database in the cloud
DB engine type: DB type you want to run (pgsql, mysql etc)
DB instance class: CPU + memory capacity of DB instance
Multi AZ: Fault tolerance / high availability
Read replica: A node a part of the db instance that only reads queries (burdens load from master)
Primary host: node within DB that handles the read / write traffic of the db
Secondary host: the backup of primary incase of failover
Aurora: cloud native engine that aws created for pgsql and mysql