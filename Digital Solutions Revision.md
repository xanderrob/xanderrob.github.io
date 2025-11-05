---
layout: default
title: Digital Solutions
# (Just the Docs extra, if you want sidebar ordering)
nav_order: 2
parent: External Revision
---

# Topics Overview
- Digital methods for exchanging data
- Complex digital data exchange problems and solution requirements
- Prototype digital data exchanges

## Top Topics

Security and cryptography
Algorithms and pseudocode
Systems modelling (DFDs)
UI/UX & visual comms

## Next:
Privacy/APP awareness
Data formats over database syntax
Networks in MC

# Pseudocode
Conventions for writing pseudocode:
**KEYWORDS** are written in bold capitals and are often words taken directly from programming languages.
For example, **IF**, **THEN**, and **ELSE**, are all words that can be validly used in most languages. **OUTPUT** and **COMPUTE** are from the language COBOL and **WRITE** is from the language Pascal.
Keywords do not have to be valid programming language words 

Variable naming schemes:
	myVariable ← use this one
	MyVariable ← or this one
	my_variable

- Capitalise reserved words
- indentations
- start/stop blocks

Example of rules: 
BEGIN
	SET x TO 0
	WHILE x < 10 DO
		INCREMENT x ✅ acceptable
		SET x TO x + 1 ✅ acceptable
		SET x = x + 1 ✅ acceptable
		x += 1 ❌ only in python - not pseudocode
	ENDWHILE
	SHOW “Done!” 
END 
## Functions

Define functions before using them in the program

BEGIN func1(x)
	…
END func1

## Selection
Single branch selection:

IF condition THEN
	…
ENDIF

**OR**
Multiple branch selection:

IF condition then
	…
ELSE
	…
ENDIF
# Algorithms
VESPA
Variables
Equations
Solve
P
Answer

Inputs/Outputs
# Data Structures
Arrays, strings, and dictionaries


# Modularisation

# Data Transfer Protocols
HTTP/HTTPS, FTP, VPN, streaming and broadcast packets

## HTTP

Hypertext transfer protocol (HTTP) is a stateless request/response protocol, which means that each message received is treated as an independent exchange between the client and the server and is not reliant on a successful login or menu selection from another web page. Each request message can be understood in isolation. The HTTP client can be a webpage, IoT device, traffic camera, mobile app or desktop app, that sends an HTTP request. An HTTP server is a web server, robot, network component or interactive media platform that responds to the HTTP request. Each HTTP request contains a method type and a Uniform Resource Identifier (URI). The HTTP response includes a success code or error code and a series of response messages containing the requested data. For example, in response to an HTTP request containing a GET method and a web page address URI, a web server HTTP response would typically contain a success code followed by the web page data. If there is no data available at the specified location then a ‘404 Not Found’ error code would be sent instead. 

## HTTPS

The ‘s’ in HTTPS stands for ‘secure’. HTTPS  is a secure version HTTP that uses Transport Layer Security (TLS) or Secure Socket Layer (SSL) protocols to encrypt the transmission using public key encryption methods. TLS is often referred to as SSL/TLS as it is essentially just a new version of SSL with some extra features. When a web page or data is requested via HTTPS, the web server will first send an SSL certificate to the browser. This contains the public encryption key to begin the data exchange. The public key is then used in an ‘SSL handshake’ to establish a secure session. The SSL handshake process is: 
1. The client node sends the SSL version number, a list of possible cipher suites that could be used and a list of possible compression settings to the server. 
2. The server node selects the most secure settings support by both client and server, and replies with the selected SSL version number, cipher, and compression settings.
3. The client node authenticates the SSL certificate and sends an encrypted message back to the server using the public key from the SSL certificate. The message contains a secret that can be used for authentication during the session. 
4. The server node uses its private key to decrypt the secret message.
5. Both client node and server node confirm that the session will be encrypted and begin exchanging encrypted data.

## FTP

File transfer protocol (FTP) is the protocol used to exchange files over the Internet. It is used by web developers to upload files to a web server. It can also be used to download files from an online server to a client machine. Due to security vulnerabilities it is blocked on most web servers. 

FTP connections are initiated with a username and password authorised to connect to the server with the FTP protocol. Once the FTP session is established, files can be exchanged freely between the client and the server. The FTP session is not encrypted. The password and all files are sent as plain text, so FTP is considered very insecure. if an encrypted connection is required, SFTP can be used instead of FTP, so that the password is not sent as plain text. Some servers offer an anonymous FTP service that allows unauthenticated access to the server. 

The address of FTP sites usually begins with ftp:// instead of http://, and ‘ftp’ instead of ‘www’, for example ‘ftp://username@ftp.example.com/’. File transfers can be requested at the command line using standard FTP commands such as ‘open’, ‘get’, ‘put’, and ‘close’. DOS-like commands such as ‘cd’, ‘dir’, ‘mkdir’, and ‘rmdir’ can be used to navigate, create and delete folders, on the FTP server. Graphical FTP software, or FTP-plugins, to web development software such as Adobe Dreamweaver, allows files to be dragged between client and server windows once an FTP session has been established.  

## VPN

A virtual private network (VPN) is an encrypted connection between two network devices. All the traffic sent between the two devices is encrypted until the connection is closed. Establishing a VPN connection is commonly referred to as ‘tunnelling’, and can be implemented with a variety of different security protocols, such as SSL at the application layer, or IPSec at the network layer. Because most VPN security protocols use public key encryption, a VPN connection ensures both data integrity and authentication during the data exchange. VPNs are used for a range of purposes, including accessing sensitive data remotely, and exchanging data securely between applications.  
# Data Exchange Methods
REST, JSON, and XML

# Encryption

## Encryption & Authentication

Authentication is the process of verifying that someone is who they say they are. A signature witnessed by a third party is a common method of authenticating that someone is eligible to take a driving test. Providing login credentials such as a username and password is a common way of authenticating a student on a school network, or a member of a gaming community. Often, the terms “one step”, or “two step” are used to identify how many levels of authentication are required at the application level before access is granted to the application. 

When exchanging data over a network, it is sometimes important to authenticate an IoT device, a software API, or a network server, to ensure they are not being impersonated in a malicious attack. A payment gateway, in particular, needs to authenticate that payment requests originate from a legitimate source. Digital signatures and application tokens are common strategies for authentication of users and devices over the internet at the network level.  

## Symmetric vs. Asymmetric Encryption

Whether a cipher is symmetric or asymmetric is to do with how the keys are generated and shared between parties. 

The key difference is that symmetric encryption is **fast but requires secure key sharing**, while asymmetric encryption is **slower but solves the key distribution problem**. In practice, modern systems often combine both approaches: asymmetric encryption is used to securely exchange a symmetric session key, and that symmetric key is then used for encrypting the actual data. This hybrid approach underpins secure protocols like **TLS/HTTPS**, balancing both efficiency and security.
![[Pasted image 20250827141552.png]]

### Symmetric Encryption

Symmetric encryption is a method where the same key is used for both encrypting and decrypting data. It is generally faster and less computationally expensive than asymmetric encryption, making it well suited for encrypting large amounts of data of securing communication channels that require speed, such as streaming or database storage. Popular symmetric algorithms include DES, AES, Blowfish, and Twofish. The main drawback is key distribution: both sender and receiver must securely share and store the same secret key. if that key is intercepted or leaked, the entire system becomes compromised.

### Asymmetric Encryption

Asymmetric encryption, also known as public key encryption, uses a pair of keys: a public key for encryption and a private key for decryption. This removes the problem of securely distributing a single shared key, since the public key can be shared openly while the private key remains secret. Common algorithms include RSA and Elliptical Curve Cryptography (ECC). Asymmetric methods are computationally heavier and slower, so they are often used for smaller data like digital signatures, authentication, or securely exchanging a symmetric session key rather than encrypting bulk data directly.

## Encryption Methods (IMPORTANT)

### TripleDES
TripleDES is a more secure version of the US government DES security protocol, and encrypts data three times using a different key for at least one of the encryption iterations. Although popular for securing financial transactions, it is slower than most other encryptions methods as the process is repeated three times. 

### Blowfish and Twofish
Blowfish and Twofish are unpatented open-source encryption algorithms. Blowfish splits up a message into blocks of 64 bits and encrypts each block individually. It is one of the faster encryption algorithms and is often used in e-commerce payment gateways and password management systems. Twofish is a very similar algorithm that uses 128 bit blocks.
### AES
The Advanced Encryption Standard (AES) uses a block cipher. It replaces DES as the US government encryption standard in 2000 and is one of the most popular and secure encryption algorithms. 

### OpenPGP
Pretty Good Privacy (PGP) uses a combination of symmetric and public key encryption. PGP uses public key encryption at the beginning of a session to exchange keys and encrypt the symmetric key. Then any messages that have to be sent during the session are encrypted using symmetric encryption. Because the session key has been encrypted using public key encryption, it can be sent securely with each message.

### RSA
In the Rivest-Shamir-Adleman algorithm (RSA), a public key is used to encrypt the message and a private key is used to decrypt it. The strength of the algorithm is attributed to the large prime numbers and keys used in the encryption calculations. However, the size of the integers also results in a slower encryption and decryption process. 

The RSA encryption process is a complicated mathematical algorithm involving prime numbers and the Euclidean algorithm. If you have ever visited a website using HTTPS, it is likely that an RSA algorithm was used to encrypt and decrypt the transmissions between your device and the secure web server. 

RSA encryption was one of the first widely used forms of **asymmetric** encryption. It was discovered by Ron Rivest, Adi Shamir, and Leonard Adleman, at the Massachusetts Institute of Technology (MIT) in the late 1970s. It works in a practical sense on the level of difficulty of completing factorisation of the product. The mathematics behind RSA is quite advanced. We will explore a simplified version of RSA.
[[RSA Algorithm]]

**MODERN CIPHERS**
![[Pasted image 20250827141430.png]]

# Privacy Principles
In Australia, the _Privacy Act_ 1988 provides legal rights and regulations relating to how personal information is collected, handled and destroyed. The act describes personal information as ‘information or an opinion, whether it is true or not, and whether recorded in a material form or not, about an individual who is reasonably identifiable’. 

Individual information, in a general sense, is any element of information that is used to describe a person or is linked to them. This includes data such as name, date of birth, and unique identifiers such as drivers license number, tax file numbers, financial account details, signatures, address and contact information, medical records, and taxation records. Data associated with this, such as sales information, logs, religious affiliations, memberships, political opinions, and other personal traits are also deemed a part of this if a person is identifiable, either directly, or indirectly from them. 

Most Australians consider information privacy to be one of their basic rights. Most, however, find it difficult to describe what privacy is and what it means to them in detail. Privacy is best explained as a legal right to control how personal information is collected, used, and handled. With evolution of data-driven technologies, there are a number of pressures working against the notion of privacy. 

The Australian Privacy Principles are a set of protocols that came into effect in 2014. The principles are:

1. Open and transparent management of personal information
2. Anonymity and Pseudonymity
3. Collection of solicited personal information
4. Dealing with unsolicited personal information
5. Notification of the collection of personal information
6. Use or disclosure of personal information
7. Direct marketing
8. Cross-border disclosure of personal information
9. Adoption, use or disclosure of government related identifiers
10. Quality of personal information
11. Security of personal information
12. Access to personal information
13. Correction of personal information

Three of the Australian Privacy Principles are closely aligned with data exchange and
open data. These are 1, 6, and 11.

# Principle of Utility
Utility can be best described as the ability of different systems to provide information in the same way to a single user.

# Usability Principles






# Ciphers

## Caesar

```
BEGIN
    INPUT message
    INPUT shiftKey
    INPUT mode   // Encryption or Decryption
    SET eMessage TO ""

    FOR EACH char IN message DO
        IF char ≠ ' ' THEN
            SET ascii TO ASCII(char)

            IF mode = "Encryption" THEN
                SET ascii TO ascii + shiftKey
                IF ascii > 90 THEN
                    SET ascii TO ascii - 26
                END IF
            ELSE
                SET ascii TO ascii - shiftKey
                IF ascii < 65 THEN
                    SET ascii TO ascii + 26
                END IF
            END IF

            SET newChar TO CHARACTER(ascii)
            ADD newChar TO eMessage
        ELSE
            ADD ' ' TO eMessage
        END IF
    END FOR

    OUTPUT eMessage
END
```

## Gronsfeld

```
BEGIN 
 # convert plainText to encrypted new word using Grosnfeld 
 # key of 312 
 INPUT plainText 
 SET length = length of plainText 
 SET keyList = [3,1,2] 
 INIT newWord 
 INIT charPos  
 INIT newChar  
 INIT alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ" 
 INIT count = 0 
 FOR i = 0 TO length-1 
   charPos = position of plainText[i] IN alphabet 
   CALCULATE newPos = (keyList[count] + charPos) MOD 26 
   newChar = alphabet[newPos] 
   ADD newChar TO newWord 
   INCREMENT count BY 1 
   IF count > 2 THEN 
     SET count = 0 
   ENDIF 
   NEXT i 
 ENDFOR 
 OUTPUT newWord 
END
```


## Vigenere Cipher

```
BEGIN 
INPUT message 
INPUT keyWord 
INPUT mode (Encryption or decryption) 
SET eMessage TO empty  
SET alphaArray TO 'ABCDEFGHIJKLMNOPQRSTUVWXYZ' 
SET keyIndex TO 0 
SET keyLength TO length of keyWord 
FOR EACH character IN message 
IF (character IS NOT 'space') THEN 
SET position TO alphaArray index FOR character 
SET shift TO alphaArray index FOR current keyWord character (keyIndex) 
IF (mode = Encryption) THEN 
SET position TO position + shift 
ELSE 
SET position TO position - shift 
ENDIF 
SET position TO position modulo 26 
APPEND alphaArray value FOR position TO eMessage 
SET keyIndex TO KeyIndex + 1 
IF (keyIndex = KeyLength) THEN 
keyIndex = 0 
ENDIF 
ELSE  
APPEND 'space' TO eMessage 
ENDIF 
ENDFOR 
OUTPUT eMessage 
END
```

