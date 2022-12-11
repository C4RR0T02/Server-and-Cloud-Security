# Securing Windows Server 2019 - Server Hardening

## Cryptography

- `Concept` of applying an `algorithm` to `plaintext` to convert it to a `cipher text`
- Most algorithms used today are publicly known
- Algorithm is secured by a `key`
- `key` is a variable in the algorithm

### Types of Cryptography

+ `Symmetric key encryption`
    + Same key is used to encrypt and decrypt the data
    + 2n keys total
+ `Public key encryption (Asymmetric)`
    + Uses key pairing
    + One key is used to encrypt and the other is used to decrypt
    + (2n - 1)/n keys total

---

### Public Key Encryption

`Case Scenario`

+ Every user has a pair of keys
+ One key is only accessible to the user (Private Key)
+ Other key is publicly accessible (Public Key)
+ Only the correct public key can decrypt the message encrypted with the public key

--- 

## Encryption File System (EFS)

Types of Keys

1. FEK (File Encryption Key)
2. User A Public Key (Sender's Key)
3. User B Public Key
4. Recovery Agent Public Key

Steps to encrypt

1. File will be encrypted with the `FEK`
2. 3 boxes to be attached to the front of the file packet
3. `FEK` is placed in each of the 3 boxes at the front of the encrypted file
4. Encrypt the 3 boxes containing the `FEK` with `User A Public Key`, `User B Public Key` and `Rexovery Agent Public Key`

### Terminology

Boxes containing `User A Public Key` and `User B Public Key` is known as `Data Decryption Field (DDF)` 

Boxes containing the `Rexovery Agent Public Key` is known as `Data Recovery Field (DRF)`

### How it works

User can decrypt the public key which can then decrypt the File packet

## Implementing EFS

1. Right click folder and select `properties`
2. Click `Advanced` on within the `General` tab
3. Click `Encrypt` and `Ok`

## Malware Protection

Malware
    
    Any type of malicious code intended to harm the environment

### Types of Malware

Viruses

    Malicious executable that are embeded into files

Worms

    Self propogating virus through the network

Trojan

    Malware in a file that is freeware

Ransomware

    Encrypts file within a system and demands a ransom for the files

Spyware

    Software that tracks the system inputs and activiteis to gather information and credentials

---

# Securing Windows Server 2019 - Secure the Network

## Common Network Security Threats

DDos attacks - Distributed Denial of Service attacks

    Using bot computers to make a request to server

Malware

    - Virus
    - Worms
    - Trojan Horses
    - Ransomware
    - Spyware

Man-in-the-middle attack

    Used to gather information by being in between the user and server

## Mitigation Techniques

1. User education
2. Mitigation of common network threats
    - DDos aware network appliances and services
    - Host based firewalls
    - Antivirus software
    - Antimalware software
    - Secure Communications

## Implementing Windows firewall and advanced security

### Domain Controller

1. Right click `Inbound Rules` and Click `New Inbound Rule`
2. Create a `Custom Rule`
3. Click the type of program
4. Set the Protocol and ports
5. Set the Scope
6. Set the Action
7. Set the Profile
8. Name the Rule

## IPSec

- Suite that allows secure, encrypted communications between two computers

### Uses for IPSec

- Authenticate and encrypt `host-to-host` traffic
- Authenticate and encrypt traffic to `specific servers`
- Use L2TP/IPSec for `VPN Connections`
- Site-to-site tunneling
- Enforce logical networks

## Connection Security Rules

- Authenticate two computers before communications
- Help to Secure information sent between two computers
- Use key exchange, authentication, data integrity and data encryption

## Firewall Rules and Connection Rules

- Firewall Rules allow traffic through but `does not authenticate or encrypt` that traffic
- Connection Rules `help to secure the traffic, only if firewall rule previously configured`

## How to configure IPSec

- GPO or firewall rule
- Predefined IPSec policies for the GPO method
    - Client (Respond Only)
    - Server (Request Security)
    - Secure Server (Requires Security)

### Implementing IPSec

#### Member Server

1. Go to Windows Defender Firewall with Advanced Security
2. Right click `Inbound Rules` and Click `New Inbound Rule`
3. Create a `Custom Rule`
4. Set the Protocol and ports
5. Set the Scope
6. Set the Action
7. Set the Profile
8. Name the Rule
9. Right click `Connection Security Rules` and Click `New Rule`
10. Set Rule type
11. Set the Endpoint
12. Set the Requirements
13. Set the Authentication Method
14. Set the Profile
15. Name the Rule

#### Domain Controller

1. Go to Windows Defender Firewall with Advanced Security
2. Right click `Connection Security Rules` and Click `New Rule`
3. Set Rule type
4. Set the Endpoint
5. Set the Requirements
6. Set the Authentication Method
7. Set the Profile
8. Name the Rule

# Securing Windows Server 2019 - Secure File Services

## Install File Server Resource Manager

### Member Server

1. Open Server Manager
2. Click `Manage` than `Add Roles and Features`
3. Install `File Server Resource Manage` from File and Storage services > File and iSCSI Services > File Server Resource Manage
4. Install and reboot the device if required
5. Click `Tools` than `File Server Resource Manager`

## Quota Management

1. Open File Server Resource Manager
2. Right Click `Quota Templates` under Quota Management
3. Click `Create Quota Template`
4. Name the Template
5. Set a limit
6. Determine the Quota (Soft Quota [Able to exceed limit] / Hard Quota [Stop at the limit])
7. Add Threshold

