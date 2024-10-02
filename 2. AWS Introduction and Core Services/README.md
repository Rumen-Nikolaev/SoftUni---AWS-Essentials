# AWS Introduction and Core Services

## Table of Contents
1. Cloud Concepts
2. Registration
3. Identity and Access Management
4. AWS CLI
5. Cost Management and Budgets

## Cloud Concepts
- **High availability**
- **Fault tolerance**
- **Disaster recovery**
- **Scalability**
- **Agility**

### High Availability
- Elimination of single points of failure
- Detection of failures as they occur
- Maintain an acceptable level of service

### Fault Tolerance
- Break one thing - service still runs
- Fault isolation
- Fault containment
- Reversion models

### Disaster Recovery
- Backup and restore
- Warm standby
- Distribution across regions

### Scalability
- **Horizontal scalability** - more instances
- **Vertical scalability** - more power

### Scalability Examples
1. **Low traffic** - Run one instance; no scaling.
2. **Higher traffic** - Potentially the same complexity; horizontal scaling.
3. **More similar traffic** - Horizontal scaling up to the limit.
4. **Complicated tasks** - Potentially the same number of instances; request for vertical scaling.
5. **Need for more power (CPU/Memory)** - Assigned to one or more instances; vertical scaling.

### CapEx vs OpEx
- **CapEx (Capital Expenditure)**
  - Paid upfront
  - Buying equipment is expensive
- **OpEx (Operational Expenditure)**
  - Recurring monthly or annual payment
  - Subscription fees

## Global Infrastructure
- 33 Geographic Regions
- 105 Availability Zones
- Serves 245 Countries

## AWS Well-Architected Framework
- **6 Pillars**
- Lenses
- Architected guidance

### Well-Architected Pillars
1. Operational excellence
2. Security
3. Reliability
4. Performance efficiency
5. Cost optimization
6. Sustainability

## AWS Console Registration
### Identity and Access Management
- Securely manage access
- Allow or deny permissions
- **Users**
- **Groups**
- **Roles**

### Users
- Represents a person or a service that interacts with AWS resources
- Unique name within the AWS account
- Can have individual security credentials

### Groups
- Collection of users
- Specify permissions for a team
- Easier to manage permissions

### Roles
- IAM Identity with specific permissions
- Can be assumed by:
  - Users
  - Services
  - Applications

### Policies
- JSON documents that define permissions
- What is allowed on which resources
- Can be attached to Users, Groups, Roles

### Permissions
- Granted through policies
- Allow or deny actions on AWS Resources

### IAM Benefits
- Granular control
- Security best practices
- Centralized management
- Audit and compliance

## AWS CLI
### Creating a User
- **AWS CLI** (Command Line Interface) for AWS
- Interact with services
- Easier to automate scripts
- Unified tool for all platforms


