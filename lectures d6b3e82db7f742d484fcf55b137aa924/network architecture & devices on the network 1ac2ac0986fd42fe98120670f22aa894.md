# network architecture & devices on the network.

1st: Yes
2nd: No
3rd: No
Formula: June 30, 2024
Start date: June 25, 2024
Status: Finish
unit/module: 2.1

### Three-Tier Architecture

- Core
    
    – The “center” of the network
    – Web servers, databases, applications
    – Many people need access to this
    
- Distribution
    
    – A midpoint between the core and the users
    – Communication between access switches
    – Manage the path to the end users
    
- Access
    
    – Where the users connect
    – End stations, printers
    

![3 tier architecture.jpg](network%20architecture%20&%20devices%20on%20the%20network%201ac2ac0986fd42fe98120670f22aa894/3_tier_architecture.jpg)

- **North-South**: Refers to traffic between external networks (e.g., user to server).
- **East-West**: Describes server-to-server communication within the same data center.

![Untitled](network%20architecture%20&%20devices%20on%20the%20network%201ac2ac0986fd42fe98120670f22aa894/Untitled.png)

![SLA.png](network%20architecture%20&%20devices%20on%20the%20network%201ac2ac0986fd42fe98120670f22aa894/SLA.png)

- Top-of-rack (ToR)
    
    switching is a network architecture in which switches are placed at the top of each server rack in a data center, providing direct connections for the servers within.
    
- A backbone network
    
     also known as a core network, is connects these LANs, allowing seamless communication between 
    
- colocation datacenter
    
    **an organization is leasing space from a third-party provider similar to a cloud-based deployment model**
    
- **Fibre Channel over Ethernet (FCoE)**
    - FCoE encapsulates and transmits FC frames over enhanced Ethernet networks.
- The Internet Small Computer System Interface (iSCSI)
    - is a storage area networking protocol used to transfer block storage from storage arrays or devices to client computers that are not directly connected to those devices.

## Networking Devices

1. **Layer 2 Switch**:
    - A Layer 2 switch operates at the data link layer (Layer 2) of the OSI model.
    - It uses MAC addresses to forward frames within a local network (LAN).
    - Unlike hubs, switches intelligently filter and forward traffic only to the relevant port, improving network efficiency.
2. **Layer 3 Capable Switch**:
    - Also known as a multilayer switch, it combines Layer 2 switching with some Layer 3 routing capabilities.
    - It can route traffic between VLANs (virtual LANs) using IP addresses.
    - May provide Power over Ethernet (PoE)
3. **Router**:
    - Operates at Layer 3 (network layer) and connects different networks (e.g., LAN to WAN).
    - Routes data based on IP addresses.
    - Provides gateway functionality, allowing devices to access external networks (like the internet).
4. **Hub**:
    - An outdated device that simply broadcasts data to all connected devices.
    - No intelligence; all devices share the same collision domain.
    - Rarely used today due to inefficiency and security issues.
5. **Access Point (AP)**:
    - Connects wireless devices (like laptops or smartphones) to a wired network.
    - Provides Wi-Fi connectivity within a specific area  ( Not a wireless router)
6. **Bridge**:
    - Connects two LAN segments (usually Ethernet) and filters traffic based on MAC addresses.
    - Imagine a switch with two  to four ports
7. **Wireless LAN Controller (WLC)**:
    - Manages multiple access points in a Wi-Fi network.
    - Centralizes configuration, security, and monitoring.
8. **Load Balancer**:
    - Distributes incoming network traffic across multiple servers to improve performance and reliability.
    - Ensures efficient resource utilization.
9. **Proxy Server**:
    - Acts as an intermediary between clients and servers.
    - Enhances security, caching, and content filtering.
10. **Cable Modem** and **DSL Modem**:
    - Convert digital data from your computer to analog signals for cable or DSL lines.
    - Provide internet access via cable or telephone lines.
11. **Repeater**:
    - Extends the range of a network by amplifying and retransmitting signals.
    - Commonly used in wireless networks.
12. **Voice Gateway**:
    - Connects traditional telephone systems (PSTN) to IP-based networks (VoIP).
    - Enables voice communication over the internet.
13. **Media Converter**:
    - Converts between different types of network media (e.g., fiber-optic to copper).
    - Bridges different network technologies.
14. **Intrusion Prevention System (IPS) / Intrusion Detection System (IDS) Device**:
    - Monitors network traffic for suspicious activity (IDS) or actively blocks threats (IPS).
    - Enhances network security.
15. **Firewall**:
    - Filters and controls traffic between networks (e.g., LAN and internet).
    - Protects against unauthorized access and threats.
16. **Networked Devices** (e.g., VoIP phones, printers, cameras):
    - These devices connect to the network for specific purposes:
        - VoIP phones: Voice communication over IP networks.
        - HVAC sensors (**heating, ventilation, and air conditioning**): Building automation and climate control.
        - IoT devices: Smart devices like refrigerators, speakers, thermostats, and doorbells.
        - Industrial control systems (SCADA): Monitor and control industrial processes.
17. **Physical Access Control Devices**:
    1. These devices manage physical entry to secure areas
18. **Voice over Internet Protocol (VoIP) Phone**:
    - **Purpose**: VoIP phones allow voice communication over IP networks (like the internet).
19. **VPN Headend**:
    - **Purpose**: The VPN headend (or VPN gateway) is the entry point for a Virtual Private Network (VPN).