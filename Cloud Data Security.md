# Cloud Data Security

## Why Protect Data at Rest

- Prevent Information Disclosure
- Prevent Data Integrity Compromise
- Prevent Accidental or Malicious Deletion
- Ensure System, hardware and software availability
- Extra layer of protection if system is compromised

## Amazon S3

- Data is private by default
- Requires Credentials to access
- Bucket policy used to grant granular access
- Consider encrypting data at rest

### Types of Access Control

- Identity-Based
    - Attached to IAM User
- Resource-Based
    - Attached to Resources
    - Indicate what user is allowed to perform on the resource
    - Used to restrict access on resource based

## Encryption

- Strong Encryption Algorithm relies on mathematical properties
- Cannot be decrypted by using any key value but the one related to the key used to encrypt the data
- Important to protect the keys

### Client-Side Encryption

- Data gets encrypted before sending it to AWS
- Data stored in an encrypted state
- Keys and algorithm known only to the client

- Amazon S3 do not play a role in encrypting / Decrypting data

- Keys stored in AWS KMS or own key within application can be used

### Server-side Encryption

- AWS encrypts data on client's behalf
- Process is transparent to user
    - Users do not see the process
    - Users do not need to manage the keys

- Service endpoint handles encryption and key management process

### S3 Server-Side Encryption Types

- SSE-C (Customer Provided Keys)
    - Keys are controlled by customer
    - Does not store encryption key provided

- SSE-S3
    - AWS manage the key
    - Encrypted data and keys stored in separate hosts

- SSE-KMS
    - AWS manage the keys
    - Envelope key is used for added protection
        - encrypting your plaintext data with a data key and then encrypting that data key with a root key

### AWS KMS

- Provide ability to create and manage key
- Use hardware security modules to protect the keys
- can be integrated with other services
- Provides the ability to set usage policy to determine which user can use keys

## Why protect data in transit

- Data that actively move from one location to another
- Risks of data in transit being exposed
    - Accidental information disclosure
    - Data integrity compromise
    - Identity compromise
        - Identity spoofing
        - Man in the middle attack

### How to protect data in transit

- Secure Sockets Layer (SSL) endpoints over Transport Layer Security (TLS) (HTTPS)
- Use Encryption
- Use Amazon Virtual Private Cloud endpoint to limit access to bucket

### Protecting remote connections to servers

#### Windows Server

- Remote Desktop Protocol (RDP)
- Establish underlying SSL/TLS connection
- Use X.509 cert
- Don't use default self signed certificate

#### Linux Servers

- Secure Shell (SSH)
- Use tunneling to protect application session in transit
- Don't allow root user to use SSH terminal
- Users login with SSH key pair and password authentication is deactivated

### AWS Certificate Manager (ACM)

- Provides single interface to manage public and private certificate
- Makes it easy to deploy certificate
- Protect and store private certificate
- Minimize downtime and outage with automatic renewals 

### AWS Certificate Manager Private Certificate Authority

- Create Private Certificate Authority hierarchies without investment and maintenance cos of operating an on-premises CA
- Can issue X.509 certificates
    - Create encrypted TLS communication channel
    - Authenticate devices
    - Cryptographically sign code
    - Implement Online Certificate Status Protocol to obtain certificate revocation status
- Used for enterprise customer building public key infrastructure in AWS cloud
- Private use in Organization
- Trusted only within the organization
- Customizable to organization internal needs

### AWS Private CA Considerations

- Hardware Security Modules (HSM)
- IAM policy for access control
- Certificate Revocation List
- Generated audit reports
