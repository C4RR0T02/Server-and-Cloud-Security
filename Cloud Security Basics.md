# Cloud Security Basics

## What is Virtualization

- Multiple systems can be ran on a single server maximizing the resources

## What is Cloud Computing

- Outsource data center operations to a cloud service provider

## Various Cloud Deployment Models

### Private Cloud

- Infrastructure provisioned for exclusive use by single organization with multiple consumers

### Community Cloud

- Infrastructure provision for exclusive use by a specific community sharing a concern

### Public Cloud

- Infrastructure provisioned for use by general public

### Hybrid Cloud

- Infrastructure comprising of two or more distinct cloud infrastructure that is unique entities

## Cloud Service Models

### Infrastructure as a Service (IaaS)

- Customer manage
    - Software
    - Operating System
    - Network within system

### Platform as a Service (PaaS)

- Customer manage
    - Software
    - Operating System Configuration

### Software as a Service (SaaS)

- Customer is just a user

## Shared Responsibility Model

### Customer Manage

- Customer Data
- Platform
- Application
- Identity and Access Management
- Operating Systems
- Network
- Firewall Configuration
- Client-data encryption
- Server-side encryption
- Networking Traffic Protection

### AWS Manage

- Compute
- Storage
- Database
- Networking
- Regions
- Availability Zones
- Edge Location

## AWS IAM

- Web Service
- Securely control access
- Used to Control who is authenticated and is authorized to use the resources

### User

Person or application

### Group

Collection of user to grant identical permissions

### Role

Identity to grant temporary permissions

### IAM Policy

Document that defines the permission
    - Level of access
    - Which resource

### Identity-based policy

Policy assigned to user

### Resource-based policy

Policy assigned to Resource

### IAM Policy Evaluation Logic

- Explicit Deny and no explicit allow is deny
- Allow is allow

