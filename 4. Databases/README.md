# Databases: Different Purposes, Scaling, and Performance

## Table of Contents
1. Recap of the Previous Session
2. Relational / SQL Databases
3. Non-relational / NoSQL Databases
4. In-Memory Databases
5. Time Series Databases

## Recap of the Previous Session
- SQS
- SNS
- SES
- Route53
- KMS and Certificates
- Tags

## Relational / SQL Databases
- **Aurora**
- **MySQL and PostgreSQL**
  - Durable in 3 AZs for the price of 1 copy
- **RDS**
  - Collection of managed DB services
  - 8 Engines
- **Redshift**

### Relational Database Service (RDS)
- Simple, fast, and predictable
- AWS handles patching, backups, and replications
- Compatible with: Aurora, MySQL, PostgreSQL
- No cost to get started
- Pay for what you consume

### What Makes RDS Good and Fast?
- General Purpose (SSD) Storage
  - 3 IOPS per GB provisioned
  - Burst up to 3,000 IOPS
- Provisioned IOPS (SSD) Storage
  - High and predictable performance
  - Provision up to 3 TB storage and 30,000 IOPS per instance

### RDS Backups
- Automated backups
- Point-in-time recoveries (PIT)
- Enabled by default
- Retention period up to 35 days
- Manual snapshots
  - Initiated by us
  - Persist until we delete them
  - Stored in S3

### How to Scale with RDS?
- Scale instances up or down
- Offload read traffic to read replicas
- Put a cache in front of RDS (ElastiCache or EC2 custom cache)

### Relational DB Management Services
- SQL - structured data and universal language
- ACID rules:
  - Atomicity
  - Consistency
  - Isolation
  - Durability

## Non-relational / NoSQL Databases
- NoSQL = Not Only SQL or Non-SQL
- Store unstructured data
- Stored in denormalized form
- Very fast responses
- Easily scalable
- Redundant copies in multiple locations

### DynamoDB Features
- Fully managed
- Collection of keys associated with values
- No query language (PartiQL)
- Indices
- DynamoDB Streams
- Single Table Design

### DynamoDB Indices
- Primary Key
- Partition Key (Hash Key)
- Composite Key (PK and Sort Key)
- Global Secondary Index
- Local Secondary Index

### DynamoDB Scan
- Examines every item in the table
- Returns all data
- Filters can be applied after the return
- Expensive on larger tables

### PartiQL
- SQL compatible query language
- SQL-like syntax for queries
- Easier for those familiar with SQL

## In-Memory Databases
- Relies on main memory
- Faster access and high-speed data retrieval

### In-Memory DB Benefits
- Speed
- Low Latency
- Scalability

### In Memory DB Drawbacks
- High memory costs
- Data could be lost
- Persistence mechanisms
- Size limitations
- Complexity of planning

### Amazon ElastiCache
- In-Memory data store and cache
- Supports Redis and Memcached

## Time Series Databases
### Amazon Timestream
- Purpose-built Time Series DB
- Fast ingestion and querying
- Cost optimization
- Integrations with Kinesis, IoT, etc.


