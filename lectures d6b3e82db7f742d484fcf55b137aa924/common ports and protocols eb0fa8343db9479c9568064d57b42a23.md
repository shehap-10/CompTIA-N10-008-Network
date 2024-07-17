# common ports and protocols

1st: Yes
2nd: No
3rd: No
Formula: June 27, 2024
Start date: June 22, 2024
Status: Hard
unit/module: 1.5

![Untitled](common%20ports%20and%20protocols%20eb0fa8343db9479c9568064d57b42a23/Untitled.png)

### What is port number and the used of those protocols

- FTP
    - File Transfer Protocol (FTP)
    - what is the different 21vs  20?
        
         port 20 is used for data transfer and port 21 for control (commands).
        
    
    Simple and efficient file transfer protocol.
    
    - **Similarity:** Similar to SFTP but less secure as it transmits data in plaintext.
- (TFTP)
    - Trivial File Transfer Protocol
    - **Port:** 69
    - **Explanation:** TFTP is used for transferring small files where security and authentication are not required.
        - **Similarity:** Similar to FTP but with less functionality and no authentication.
- SFTP
    
    Secure File Transfer Protocol (SFTP)
    
    - **Port:** 22
    - **Explanation:** SFTP uses SSH to securely transfer files between networked hosts.
    - **Similarity:** Similar to FTP but uses SSH for encryption, making it more secure.
- SSH
    - Secure Shell (SSH)
    - **Port:** 22
    - **Explanation:** SSH is used for securely logging into a remote machine and executing commands encrypted communication.
    - **Similarity:** SSH is similar to Telnet but adds encryption for security.
- Telnet
    - **Port:** 23
    - **Explanation:** Telnet is used for logging into remote systems via a text-based interface.
- (SMTP) vs SMTP TLS
    - Simple Mail Transfer Protocol
    - **Port:** 587
        - SMTP over TLS
    - **Port:** 25
    - **Explanation:** SMTP is used for sending emails between servers.
    - **Similarity:** Works alongside POP3 and IMAP which handle email retrieval.
- (DNS)
    - Domain Name System
        - **Port:** 53
        - **Explanation:** DNS translates domain names (human-readable) into IP addresses.
- (DHCP)
    - **Ports:** 67/68
        - request 68 for node
        - to 67 router / servers DHCP
    - Dynamic Host Configuration Protocol
    - **Explanation:** DHCP automatically assigns IP addresses to devices on a network.
- (HTTP)
    - **Port:** 80
    - Hypertext Transfer Protocol
    - **Explanation:** HTTP is used for transferring web pages on the internet.
    - **Similarity:** Similar to HTTPS but without encryption.
- Network Time Protocol (NTP)
    - Network Time Protocol
    - **Port:** 123
    - **Explanation:** NTP synchronizes the clocks of devices on a network.
- (POP3)
    - Post Office Protocol v3
    - **Port:** 110
    - **Port:** 995
        - POP3 over SSL secures email
    - **Explanation:** POP3 is used by email clients to retrieve emails from a server usually downloading and deleting from the server.
- (IMAP)
    - Internet Message Access Protocol
    - **Port:** 143
    - **Port:** 993
        - IMAP over SSL secures email
    - **Explanation:** IMAP is used by email clients to retrieve and manage email from a server.
    - **Similarity:** Similar to POP3 but supports email synchronization and server-side management.
- (SNMP)
    - Simple Network Management Protocol
    - **Ports:** 161 VS 162
        - **Port 161:** Used by SNMP agents, which are the devices being monitored or managed
        - **Port 162:** Used by SNMP managers, which receive alerts (traps) and notifications from the agents.
    - **Explanation:** SNMP is used for network management and monitoring.
- (LDAP) +S
    - Lightweight Directory Access Protocol
    - **Port:** 389
    - **Port:** 636
        - LDAP over SSL for secure directory access.
    - **Explanation:** LDAP is used for accessing and maintaining distributed directory information services.
    - **Similarity:** Similar to LDAPS but without SSL encryption.
- (HTTPS)
    - Hypertext Transfer Protocol Secure
    - **Port:** 443
    - **Unique Objective:** Secure web communication using SSL.
- (SMB)
    - Server Message Block
    - **Port:** 445
    - **Explanation:** SMB is used for providing shared access to files, printers, and serial ports between nodes on a network.
    - **Similarity:** Similar to FTP but focuses on network resource sharing.
- Syslog
    - **Port:** 514
    - **Explanation:** Syslog is used for message logging from network devices.

### Database

- Structured Query Language (SQL) Server
    - **Port:** 1433
    - **Explanation:** SQL Server (Microsoft SQL Server) is used for managing and querying relational databases.
- SQLnet
    - **Port:** 1521
    - **Explanation:** SQLnet is Oracle's protocol for connecting to Oracle databases.
- MySQL
    - **Port:** 3306
    - **Explanation:** MySQL is an open-source relational database management system.
- (RDP)
    - Remote Desktop Protocol
    - **Port:** 3389
    - **Explanation:** RDP is used for remote desktop connections to manage a computer from another device provides a graphical interface.
- Session Initiation Protocol (SIP)
    - **Ports:** 5060 (unencrypted) vs 5061 (encrypted with TLS)
    - **Explanation:** SIP is used for initiating, maintaining, and terminating real-time sessions including voice, video, and messaging applications.
    - **Unique Objective:** Real-time communication sessions.
- (ICMP)
    - Internet Control Message Protocol
    - Provides feedback about network issues such as unreachable hosts or network congestion.
    - Unlike TCP and UDP, ICMP is not used for data transmission but for control messages and error reporting.
- (GRE)
    - Generic Routing Encapsulation
    - **Explanation:** GRE is used to encapsulate a wide variety of network layer protocols inside virtual point-to-point connections.
    – The “tunnel” between two endpoints
    • Encapsulate traffic inside of IP Two endpoints appear to be directly
- Internet Protocol Security (IPSec)
    - **Explanation:** IPSec is a suite of protocols for securing IP communications by authenticating and encrypting each IP packet in a communication session.
    - **Unique Objective:** Ensures secure IP communications through encryption and authentication.
    - **Similarity:** Can be used with AH and ESP to provide comprehensive security features.
- Authentication Header (AH)
    - **Explanation:** AH is part of IPSec and provides data integrity, authentication, and anti-replay protection for IP packets.
- Encapsulating Security Payload (ESP)
    - **Explanation:** ESP is part of IPSec and provides data confidentiality, as well as optional data integrity, authentication, and anti-replay protection.