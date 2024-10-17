# Homework: Databases - Different Purposes, Scaling, and Performance

## Questions and Answers

1. **What is Amazon RDS and which databases does it support?**

   Amazon RDS (Relational Database Service) is a managed database service provided by AWS that simplifies the setup, operation, and scaling of relational databases in the cloud. It supports several database engines, including:
   - Amazon Aurora
   - MySQL
   - PostgreSQL
   - MariaDB
   - Oracle
   - Microsoft SQL Server

2. **What are the benefits of Multi-AZ deployments?**

   Multi-AZ deployments provide enhanced availability and durability for RDS instances. Benefits include:
   - Automatic failover to a standby instance in case of an outage.
   - Data redundancy across multiple availability zones.
   - Automated backups that are stored in a separate location.
   - Improved availability during maintenance operations.

3. **What are read replicas and why are they used?**

   Read replicas are copies of the primary database instance that allow for read-only access to the database. They are used to:
   - Offload read traffic from the primary instance, improving performance.
   - Scale read operations horizontally to support large volumes of queries.
   - Provide increased availability for read operations.

4. **When an RDS instance is deleted, is there anything left that could incur additional costs?**

   When an RDS instance is deleted, automated backups, manual snapshots, and read replicas may still exist and incur costs. If a final snapshot is created during the deletion process, it will persist until explicitly deleted, potentially resulting in ongoing storage costs.

5. **What are the differences between DynamoDB and RDS?**

   The primary differences between DynamoDB and RDS include:
   - **Data Model**: RDS uses a relational data model, while DynamoDB uses a NoSQL, key-value and document data model.
   - **Scalability**: DynamoDB is designed for horizontal scalability, while RDS provides vertical scalability with read replicas.
   - **Query Language**: RDS uses SQL for queries, while DynamoDB primarily relies on key-value access and PartiQL for querying.
   - **Data Structure**: RDS enforces a schema, whereas DynamoDB allows for flexible schemas.

6. **What is the difference between Partition Keys and Sort Keys?**

   - **Partition Key**: The primary key that determines the partition in which the item is stored. It is used to distribute data across multiple partitions to ensure balanced storage and access.
   - **Sort Key**: An optional secondary key that allows for sorting items with the same partition key. It enables the organization of items within the same partition and allows for range queries on the sort key.

