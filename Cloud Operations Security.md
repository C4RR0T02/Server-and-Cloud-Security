# Cloud Operations Security

## Security Operations Function

- `Detect`, `respond` to, `recover` from active attacks on enterprise assets

Security Operations should
- Reactively respond to attacks detected by tools
- Proactively hunt for attacks that slip past reactive detections

## What is Logging

- Collection and recording of activity and event data
    - provided by services
- Information logged varies from service conducting the logging
- Common log elements
    - Date and time of event
    - origin of event
    - identity of resource accessed

## Why is logging important

- Provides record of events
    - troubleshooting
    - auditing
    - record keeping
    - incident response and remediation

- Logs required for compliance
    - HIPAA
    - GDPR
    - LGPD

## What is monitoring

- Continuous verification of security and performance of resources, applications and data
- AWS provide services that give visibility to spot issue before it impacts the operation
    - AWS CloudTrail
    - Amazon Cloudwatch
    - Amazon EventBridge
    - AWS X-Ray

## AWS CloudTrail

- Enable governance and compliance and operational and risk auditing of AWS account
- Records action by user, role or AWS Service as events
- Provides visibility of events in the CloudTrail Console
- Used to view, search, download, archive, analyze, and respond to account activity across the AWS infrastructure

### API Security-relevant information

- Records important information about each API call
    - Name of API
    - Identity of the caller
    - Time of API call
    - Originating location of request
    - Request parameters
    - Response elements

- Track changes to resources
    - Creation
    - Modification
    - Deletion

## Amazon CloudWatch

- monitoring and observability service
- Provide unified view of operational health of resources,applications and services
- collect metrics in AWS cloud and on premies
- Used for infrastructure monitoring and troubleshooting
- provide ability to customize logs and events

## Whats the difference between CloudTrail and CloudWatch

CloudTrail
- Continuously monitor and logs user activities
- Useful for compliance auditing, security analysis and troubleshooting
- Determine Who perform What unauthorized action and When the did it

CloudWatch
- Continuously monitor resources and application performance
- Useful in detecting anomalies in service behaviors, setting alarms and discovering insights
- Alerts user when an issue occurred due to unauthorized action

Can create custom CloudWatch dashboard, alarms and notification for key metrics for specific CloudTrail events 

## Monitoring and Logging Best Practices

- Define organization requirement for logs, alerts, and metrics
- Configure service and application logging throughout the workload
- Analyze log centrally

## Incident Recognition and Response

- Set of information security policies and procedures to use to identify, contain and eliminate cyber attacks
- Help organization quickly detect and stop attacks
- Help to minimize damage and prevent future attacks

### Recognizing incidents

- Not all events need immediate remedy
    - Logging in from remote location
    - Failing hard drive that is still fully operational
    - Employee trying to access resources they shouldn't access

### Phase 1: Discovery and Recognition

- Identifying, logging, and categorizing the incident
- Incident notification and escalation
- Investigation and diagnosis

### Phase 2: Resolution and Recovery

- Forensic Isolation
    - Reproduce the bug
- Stage a fix
- Deploy the fix
- Incident Closure

Automate this processes where possible in a safe environment to fine-tune the incident response process

