# Advanced Services Overview

## SoftUni Team

### Technical Trainers

### Agenda
1. Review of Previous Session
2. Storage Solutions
3. Simple Queue Service and Related Concepts
4. Security Measures on AWS
5. AWS Amplify
6. Tagging in AWS

---

## Review of Previous Session
- Registration Process
- Identity and Access Management (IAM)
- Command Line Interface (CLI)
- Billing and Budgeting

---

## Storage Solutions
- Understanding Object, File, and Block Storage
- Data Migration Strategies
- Hybrid Cloud Storage Solutions
- Managed Cloud Transfer Services
- Disaster Recovery and Backup Techniques

### Storage Options
- **Amazon S3 (Simple Storage Service)**
  - Stores objects in "buckets"
  - Offers exceptional durability (99.999999999%)
  - Free Tier includes 5GB of storage
  - Capable of hosting static websites

### Object Storage with S3
- **AWS Snow Family**
  - Includes Snowcone, Snowball, and Snowmobile
- **Data Transfer Solutions**
  - AWS DataSync and AWS Storage Gateway
  - AWS Transfer Family

---

## Simple Queue Service and Related Concepts
- A fully managed queuing service
- FIFO (First In, First Out) messaging
- High reliability for large data volumes
- Helps in decoupling application components
- Ensures message order integrity

### Simple Notification Service
- Managed Pub/Sub service for applications
- Enables app-to-person notifications via:
  - Email
  - SMS
  - Push notifications for mobile apps
  - Application-to-application notifications
- Automated messaging capabilities

### Simple Email Service
- Email service provider for:
  - Automated messages
  - Newsletters
  - Domain registration services

### Hands-On Activity: Working with Queues

---

## Security in AWS
- **Route 53**
  - DNS service to direct end users to applications
  - Manage network traffic efficiently

- **AWS Key Management Service (KMS)**
  - Manages cryptographic keys
  - Facilitates signing operations

- **AWS Certificate Manager**
  - Handles certificates for TLS and SSL

- **Amazon Cognito**
  - Manages user identification and access for applications
  - Supports user pools and identity pools
  - Allows for custom authentication methods

### JSON Web Tokens (JWT)
- Internet standard for securely transmitting information
- Encrypted JSON format containing claims and user data

---

## AWS Amplify
- Streamlines full-stack application development
- Designed for web and mobile applications
- Automates development workflows
- Ideal for proof of concepts, although more complex projects may present challenges

### Key Features of AWS Amplify
- Backend as a Service (BaaS)
- Integration with Amplify CLI and Cloud Development Kit (CDK)
- Monitors user activity and compliance
- Can trigger other AWS services for various use cases
- Assists in investigating issues and ensures organizational compliance

---

## Amazon CloudFront
- Content delivery network for caching and dynamic content delivery
- Supports live and on-demand video streaming

---

## Tagging in AWS
- Key-value pairs for resource organization
- User-defined and auto-generated tags by some AWS services

### Use Cases for Tagging
- Financial tracking and cost allocation
- Operational management and support
- Data security and compliance

### Hands-On Activity: Working with CloudTrail and Tags

---

## Homework Assignments
- Investigate the cost of AWS CloudTrail and estimate usage until charges reach $1.
- Create a new Trail.
- Set up an S3 Bucket and upload a text file.
- Tag the uploaded file.
- Disable logging for the Trail.
- Analyze the Trail logs in CloudWatch.
- Identify patterns in the logs and describe them.
- Discuss potential benefits of the data gathered from the logs.

