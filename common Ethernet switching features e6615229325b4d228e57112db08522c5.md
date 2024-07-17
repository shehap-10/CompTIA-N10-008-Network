# common
Ethernet switching features

1st: No
2nd: No
3rd: No
Formula: June 28, 2024
Start date: June 27, 2024
Status: 2end
unit/module: 2.3

Explore

[https://www.bing.com/th?id=OSK.b2fdef42858ce025b3a00418c0ba42f7&pid=cdx&w=320&h=189&c=7&rs=1](https://www.bing.com/th?id=OSK.b2fdef42858ce025b3a00418c0ba42f7&pid=cdx&w=320&h=189&c=7&rs=1)

Certainly! Let’s dive into each of these networking concepts in depth:

1. **Data Virtual Local Area Network (VLAN)**:
    1. Segment think IP address layer 3
    - A VLAN is a logical subnetwork of devices within a broadcast domain. It is created by partitioning network switches or using network management software.
    - VLANs allow you to group devices (such as computers, servers, or IP phones) into separate segments, even if they share the same physical network.
    - Example: Creating a VLAN for HR department computers to isolate their traffic from other departments.
2. **Voice VLAN**:
    - Voice VLANs are used for IP phones (e.g., VoIP phones) and separate voice traffic from data traffic.
    - IP phones often connect to computers, so a voice VLAN ensures that voice and data traffic remain separate.
3. **Port Configurations**:
    - Port configurations refer to settings applied to individual switch ports.
    - Common configurations include access ports (for connecting end devices) and trunk (Multiple VLAN in one cable) ports (for VLAN traffic).
4. **Port Tagging (802.1Q)**:
    - 802.1Q is a protocol for tagging Ethernet frames with VLAN information. (VLAN id)
    - Tagging allows switches to distinguish between different VLANs on the same physical link.
        
        A non-tagged frame is on the default VLAN Also called the native VLAN
        
5. **Port Aggregation (Link Aggregation)**:
    - Link aggregation combines multiple physical links into one logical link.(Multiple interfaces acts like one big interface) provides redundancy..
6. **Duplex, Speed, and Flow Control**:
    - **Duplex**: Determines whether communication is full-duplex (both directions simultaneously) or half-duplex (one direction at a time).
    - **Speed**: Refers to the data rate (e.g., 1 Gbps, 10 Gbps) supported by the port.
    - **Flow Control**: Mechanism to manage data flow and prevent congestion.
7. **Port Mirroring**:
    - Port mirroring copies network traffic from one port to another for monitoring or analysis.
    - Useful for troubleshooting, security monitoring, or network analysis.
    
    Certainly! Let’s delve into each of these networking concepts in depth:
    
    1. **Port Security**:
        - **Definition**: Port security is a feature in network switches that blocks unknown wired devices from gaining access to a network by learning the MAC addresses of connected devices of each port
    2. **Jumbo Frames**:
        - **Definition**: Jumbo frames are Ethernet frames with more than 1500 bytes of payload (commonly 9000 bytes). Increases efficiency by reducing overhead and CPU cycles.
    3. **Auto-Medium-Dependent Interface Crossover (MDI-X)**:
        - **Definition**: Auto-MDI-X automatically detects and configures the appropriate cable type (straight-through or crossover) for Ethernet connections.
    4. **Media Access Control (MAC) Address Tables**:
        - **Definition**: MAC address tables (also called Content Addressable Memory or CAM tables) are used by Ethernet switches to determine where to forward traffic within a LAN.
    5. **Power over Ethernet (PoE)**:
        - PoE delivers DC power over Ethernet cabling, allowing devices like wireless access points and IP cameras to be powered via the same cable used for data.
            
            Power provided at the switch
            – Built-in power - Endspans
            – In-line power injector - Midspans
            
        - Power modes
        – Mode A - Power on the data pairs
        – Mode B - Power on the spare pairs
    6. **Spanning Tree Protocol (STP)**:
        - **Definition**: STP prevents loops in Ethernet networks by dynamically blocking redundant paths.
        - **How It Works**:
            - Elects a root bridge and selects the best path to reach it.
            - Blocks redundant links to prevent loops.
            - Reacts to topology changes.
        - **Related Concepts**:
            - **BPDU (Bridge Protocol Data Unit)**: Messages exchanged by switches.
            - **Root Bridge**: Central switch in the STP topology.
    7. **Carrier-Sense Multiple Access with Collision Detection (CSMA/CD)**:
        - is an early Ethernet protocol that manages access to a shared communication medium in (**Half-Duplex**) Avoids data collisions by detecting carrier signals and adjusting transmission.
        - **How It Works**:
            - Devices listen for carrier signals before transmitting. If the medium is free, the device transmits its data.
            - **Collision Detection**: If two devices transmit simultaneously, a collision occurs. Each device detects the collision. devices stop transmitting, wait for a random period (back off), and then attempt to transmit again
    
    - Address Resolution Protocol (ARP)
        - Adds unknown MAC addresses to the MAC address table
        - ARP is a crucial protocol in the Data Link Layer of the OSI model.
        - ARP translates that IP address into the corresponding MAC address.
    - Neighbor Discovery Protocol
        - **Duplicate Address Detection (DAD)** is a process used in IPv6 networks to ensure that there are no duplicate IP addresses assigned to different network devices
        - Discover routers: Router Solicitation (RS) and Router Advertisement (RA)[Router Advertisement (RA) ](../Self%20Study%20fe516e7f21b1429b8722398814013d86/course%206de301d2d53c496d9ba4087260558b02/Cisco%208635094e378e434989070f76f710eff3/Cisco%20Courses%2059ab3506ef82497ead134f5f0a902b2a/CCNA1%20f46d23cb3f634bc6910698ac5abbea1b/lectures%20bb6190317baa4ebc9d87898c87434ee5/IPv6%20Addressing%20fa9cd6f9e68342d8a8c92e6540ea87bf.md)
        - No broadcasts Operates using multicast with ICMPv6