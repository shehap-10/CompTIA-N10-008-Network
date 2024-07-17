# Untitled

1st: No
2nd: No
3rd: No
Status: 2end
unit/module: 4.1

- Confidentiality, integrity, availability (CIA)
    - Integrity
        
        
        • Data is stored and transferred as intended
        – Any modification to the data would be identified
        • Hashing
        – Map data of an arbitrary length to data of a fixed length
        • Digital signatures
        – Mathematical scheme to verify the integrity of data
        • Certificates
        – Combine with a digital signature to verify an individual
        • Non-repudiation
        – Provides proof of integrity, can be asserted to
        
    - Confidentiality
        
         Certain information should only be known
        
        to certain people
        • Encryption
        – Encode messages so only certain people can read it
        • Access controls
        – Selectively restrict access to a resource
        • Steganography
        – Conceal information within another piece of information
        – Commonly associated with hiding information in an image
        
    - Availability
        
        
        • Information is accessible to authorized users
        – Always at your fingertips
        • Redundancy
        – Build services that will always be available
        • Fault tolerance
        – System will continue to run, even when a failure occurs
        • Patching
        – Stability
        – Close security holes
        
    
1. **Threats**:
    - **Internal Threats**: Risks from within an organization, such as disgruntled employees.
    - **External Threats**: Risks from outside the organization, like hackers or malware.
    1. **Vulnerabilities**:
        - **Common Vulnerabilities and Exposures (CVE)**: Known database security flaws.
        - **Zero-day**: Unpatched vulnerabilities exploited by attackers
    2. **Exploits**: Techniques used to take advantage of vulnerabilities.
    3. **Least Privilege**: Users should have minimal access rights necessary for their tasks.
    4. **Role-Based Access Control**: Permissions based on job roles.
    5. **Zero Trust**: Assume no one is trustworthy; verify all access requests
    6. **Defense in Depth**:
        - **Network Segmentation**: Dividing networks to limit lateral movement.
        - **Perimeter Network (DMZ)**: Isolated network for public-facing services.
        - **Separation of Duties**: Different people handle different tasks.
        - **Network Access Control**: Regulates network access.
        - **Honeypot**: Lures attackers away from critical systems.
        1. **Risk Management**:
            - **Security Risk Assessments**: Identifying and assessing risks.
            - **Threat Assessment**: Evaluating potential threats.
            - **Vulnerability Assessment**: Identifying weaknesses.
            - **Penetration Testing**: Simulating attacks to find vulnerabilities.
            - **Posture Assessment**: Evaluating security posture.
            - **Business Risk Assessments**: Assessing business impact.
            - **Process Assessment**: Evaluating security processes.
            - **Vendor Assessment**: Assessing third-party security.
            
            1. **Security Information and Event Management (SIEM)**: Collects and analyzes security logs and events.
            
    

### Authentication methods

- **Multifactor Authentication**: Requires multiple forms of verification.
- Authentication services
    - RADIUS
- TACACS
    - Authentication protocol for network devices. TACACS+ - Probably a Cisco device
        
        Terminal Access Controller Access-Control System
        – Remote authentication protocol
        – Created to control access to dial-up lines to ARPANET
        
- LDAP
- 
- Kerberos
• Network authentication protocol Authenticate once, trusted by the system

SSO with Kerberos
• Authenticate one time
– Lots of backend ticketing, uses cryptographic tickets
• No constant username and password input! - Save time
• Only works with Kerberos
– Not everything is Kerberos-friendly
• There are many other SSO methods
– Smart-cards, SAML, etc.