# Securing Windows Server 2019

## Cryptography

- `Concept` of applying an `algorithm` to `plaintext` to convert it to a `cipher text`
- Most algorithms used today are publicly known
- Algorithm is secured by a `key`
- `key` is a variable in the algorithm

### Types of Cryptography
+ `Symmetric key encryption`
    + Same key is used to encrypt and decrypt the data
+ `Public key encryption (Asymmetric)`
    + Uses key pairing
    + One key is used to encrypt and the other is used to decrypt

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

