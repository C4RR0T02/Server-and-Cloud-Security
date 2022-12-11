# Server Security Basics

## Objectives
- [ ] Server Roles
- [ ] Server Attack 
- [ ] Vectors
- [ ] Defense-in-Depth
- [ ] Disaster Recovery

---

## Common Network Modules

1. Peer-to-Peer (No Server)
2. Client-Server (also known as Server-based)

## What is a Server?

- Computer program or machine that waits for request from other machine
- Typically process data
- Purpose is to share data / hardware / software resources among clients
- Client-Server model
- Client run on same computer or conect to server over the network

## Security

- Confidentiality
    - Limit access and disclosure to authorised users
    - Prevent access to unauthorised people
- Integrity
    - Maintain data consistency
    - Preserve data at rest and in transit
- Availability
    - Able to access information when needed

## Server Roles

- Servers are deployed to offer services that provide business value to the organisation
- Installation, configuration, management of server roles vary depending on the OS version
- Uses Add Roles and Features Wizard for role addition in Window's Server

## Common Windows Server Roles

### Web Server
- Provide access to information users connect to through the web browser
- Uses HTTP/HTTPS as transfer mechanism

### Application Server
- Server users connect to and run the application
- Middle tier of three tier architecture to accept user request to application and connect to the database server

### Database Server
- Runs database software (MySql, MariaDB, etc...)
- Contain information stored in the database
- Users able to query database

### File Server
- Used to store files accessible by network users

### Network Services Server - DHCP
- Dynamic Host Configuration Protocol
- Server used to automate IP configuration to devices
- Responds to broadcast based request for configuration
    - Offer IP address
    - Subnet mask
    - default gateway

### Netwok Service Server - DNS
- Domain Name System
- Resolve device and domain name to IP address
- Resolve IP address to device and domain name

### Diretory Services Server
- Accepts and verify credentials of user
- Example: Active Directory Domain Services (AD DS)
- Act as core directory service for an organisation
    - Manage hierarchial relationship between network objects

## Server Attack Vectors

### Compromised / Weak Credentials
- Username and Password most common access credentials
- Exposed through 
    - Data Leaks
    - Phishing Scam
    - Malware
- Give attacker unfettered (unlimited) access when lost / stolen / exposed 
- Reduce risk of leak in credentials resulting in security incidents by
    - Password Manager
    - Two Factor Authentication
    - Multi Factor Authentication
    - Biometrics

### Poor Encryption
- Use SSL Certificate
    - Prevent Man-in-The-Middle Attack
    - Protect Confidentiality of data being transmitted
- Use Strong encryption for
    - Data at rest
    - Data in transit

### DoS / DDoS Attack
- Attack that prevent system from processing or responding to legitamate traffic
- Transmit many data packets to flood the server traffic
- Other forms focus on exploitation of known faults or vulnerabilities of OS, service or application
- Exploiting the fault often result in
    - System crash
    - 100% CPU utilization

### Botnet and DDoS
- Set of computers that is infected by a control program
- Enable attacker to collectively exploit the computer to mount attack
- Used to coordinate DoS attacks
- Infected machines called zombies / drones
- Unaware that computer is used for nefarious purpose

### SYN Flood Attack
- Exploit handshake process of TCP connection
- Usual Process
    - Client send a SYN packet to server to initiate connection
    - Server responds with initial SYN/ACK packet to acknowledge communication
    - Client returns ACK packet to acknowledge receipt of the packet
- Created by leaving connection half open
    - Sends a spoofed SYN packet
    - Server tries to respond but unable to reach client
- Server continuously leaves open connnections waiting for the connection to timeot before freeing the port

### Ping Flood
- Flood victim with ping request
- Very effective when launched by zombies in a botnet (DDoS)
- System gets ocerwhelmed trying to answer ping request
- Common Mitigation
    - Block ICMP traffic
    - Use Active intrusion detection system
        - Modify environment and block ICMP traffic during the attack

### Ping of Death
- Use oversized ping packet
- Usually 32 / 64 byte
- Sends 64 KB sized ping packet
    - Bigger than many systems can handle

### Mitigation Techniques for DDoS
- Multi-level protection strategies
- Intrusion Prevention, Threat Management Systems, firewall
- Update system to mitigate loopholes

## Defense-in-Depth
- Layered security seen as best protection for system security
- To fully compromise te system, attacker must get past multiple security control
    - Provide control diversit
- Reduce potential attack surface
    - Make it more likely the attack will be prevented

## Disaster Recovery
- Can be caused by natural disasters, security issues, power outages
    - Earthquake / Fire
    - Technology Failure
    - System Incompatibilities
    - Human error
    - Cyber Attacks
- Includes company's procedue and policy to recover from such events
- Organisations sensitive to risk of disaster will develop effective and documented Disaster Recovery Plan (DRP)
    - Identify scenarios of natural and non natural disaster and options for protecting system
    - Identify task, resources and responsibility for responding to the disaster
    - Train staff on the planning procedure and how to react

## Backup Types
- Made for security
- For restoration of original if lost or damaged

1. Full
    - All selected data regardless of when it was previously backed up
    - Requires the most time to back up
    - Restores in the fastest time
    - Take the latest full backup to recover all the data
2. Incremental
    - New files and files modified since last full backup
    - Requires least amount of time to back up
    - Restores the slowest
    - Takes the initial full back up and each set of incremental backup after the initial full backup to recover all data
3. Differential
    - All data modified since the last full backup
    - Moderate back up time
    - Moderate restore time
    - Takes the initial full back up and the latest differential backup to recover all data

