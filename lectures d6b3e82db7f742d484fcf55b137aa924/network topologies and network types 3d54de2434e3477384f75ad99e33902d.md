# network topologies and network types

1st: Yes
2nd: No
3rd: No
Formula: June 24, 2024
Start date: June 19, 2024
Status: 2end
unit/module: 1.2

## Topology types

- Mesh
    
    every device is connected to every other device in the network.
    
    ![Untitled](network%20topologies%20and%20network%20types%203d54de2434e3477384f75ad99e33902d/Untitled.png)
    
- Hybrid Topology
    - A combination of two or more different types of topologies (e.g., star-bus, star-ring).
    
    ![Untitled](network%20topologies%20and%20network%20types%203d54de2434e3477384f75ad99e33902d/Untitled%201.png)
    
- Ring Topology
    - Devices are connected in a circular fashion, with each device having exactly two neighbors.
    
    ![Untitled](network%20topologies%20and%20network%20types%203d54de2434e3477384f75ad99e33902d/Untitled%202.png)
    
- Bus Topology
    
    All devices share a single communication line or cable
    
    ![Untitled](network%20topologies%20and%20network%20types%203d54de2434e3477384f75ad99e33902d/Untitled%203.png)
    
- Star/Hub-and-Spoke Topology
    - All devices are connected to a central hub or switch.
    
    ![Untitled](network%20topologies%20and%20network%20types%203d54de2434e3477384f75ad99e33902d/Untitled%204.png)
    

### Wireless topologies

- What is Ad Hoc Networking
    
    does not rely on infrastructure, such as routers or wireless access points. Instead, each node participates in routing by forwarding data for other nodes.
    
    ![Untitled](network%20topologies%20and%20network%20types%203d54de2434e3477384f75ad99e33902d/Untitled%205.png)
    

## Network type

- Peer-to-peer
    
    A network where all devices (peers) share resources and communicate directly with each other without a central server.
    
    Each device can act as both a client and a server.
    
- Client-server
    - A network where clients (computers) request resources or services from a central server.
- (LAN)
    - Local area network:
        - A network covering a small geographical area, like a single building or campus.
        - Limited to a local area with high-speed connectivity.
- (MAN)
    - Metropolitan area network
        - A network covering a city or a large campus.
        - Larger than a LAN but smaller than a WAN.
        - Connects multiple LANs within a metropolitan area.
        - Often used by cities or large institutions.
- (WAN)
    - Wide area network:
        - A network that spans a large geographical area, often a country or continent.
        - Lower data transfer speed compared to LANs and MANs.
- (WLAN)
    - Wireless local area network
        - A LAN that uses wireless technology (Wi-Fi) to connect devices.
- (PAN)
    - Personal area network:
        - A network for connecting devices within a few meters, typically around an individual.
        - Uses technologies like Bluetooth, USB, or infrared.
        - Connects personal devices like smartphones, laptops, and wearables.
- (CAN)
    - Campus area network
        - A network that connects multiple buildings within a campus, such as a university or corporate campus.
        - Larger than a LAN but smaller than a MAN.
- (SAN)
    - Storage Area Network What is it?
    - A **Storage Area Network (SAN)** is a specialized, high-speed network that provides access to storage devices.
    - How is it used?
        - SANs are used to connect servers to storage devices (like disk arrays and tape libraries) in a way that makes the storage appear like it is directly attached to the server.
- (MPLS)
    - Multiprotocol label switching:
        - MPLS networks are private and managed by service providers, ensuring secure and reliable performance.
        - MPLS operates between OSI Layer 2 (data link layer) and Layer 3 (network layer), often referred to as a layer 2.5 protocol.
        - a telecommunications routing technique that directs data from one node to the next based on labels rather than network addresses.
        - such as videoconferencing or VoIP calls, due to its ability to reduce latency and improve quality of service (QoS).
- (SD-WAN)
    - Software-Defined Wide Area Network
        - uses software to manage wide area network connections between different locations.
        - is an automated, programmable network  WAN circuit priority. It allows companies to efficiently connect users to applications using various transport services like MPLS, LTE, and broadband internet12. SD-WAN simplifies management, improves performance, and lowers operational costs for multisite deployments.
- (mGRE)
    - Multipoint Generic Routing Encapsulation
        
        ![Untitled](network%20topologies%20and%20network%20types%203d54de2434e3477384f75ad99e33902d/Untitled%206.png)
        
        - is a tunneling protocol used to create virtual private networks (VPNs) over the internet.
        - mGRE encapsulates data to securely send it over public networks as if it were on a private network.

- Demarcation point
    
    is the physical point where a telecommunications company’s public network ends and the customer’s private network begins.
    
- Smart Jack Network Interface Unit (NIU)
    - type of Network Interface Device (NID) that provides a physical interface between the service provider's network and the customer's premises. It includes advanced diagnostic capabilities to help in managing and troubleshooting network connections
    - more
        
        **Telecom Service Provider**: A telecom company provides internet and phone services to a business. They install a SmartJack at the business's premises to connect the company's internal network to the provider's external network. If the business experiences connectivity issues, the provider can perform remote diagnostics using the SmartJack, conduct loopback tests to check the integrity of the connection, and monitor signal quality to identify and resolve the problem without needing to send a technician on-site.
        

## virtual network concepts

- **vSwitch**:
    
     It helps manage the data traffic between different virtual machines (VMs) on the same network, making sure that each VM gets the data it needs without any confusion.
    
- **Virtual Network Interface Card (vNIC)**:
    
     Imagine a vNIC as a virtual door that allows your VM to connect to the internet or other networks. It’s like having a unique address for your VM, so it can send and receive data just like a real computer would.
    
- **Network Function Virtualization (NFV)**:
    
    is like having a set of virtual tools that you can use to build or fix your network. Instead of using separate physical devices for each task, NFV lets you use software to perform these functions, such as routing, load balancing, or firewalling
    
- **Hypervisor**:
    
    It’s the software that creates and manages all the VMs, giving each one its own space and resources to run programs and store data.
    

### Provider Links

- **Satellite**
    - The provider sends your internet request up to a satellite orbiting Earth, and the satellite sends it back down. It’s great for remote areas but can be slow (250 ms up, 250 ms down) and have delays because of the long distance the signal travels.
- **Digital Subscriber Line (DSL)**:
    
    DSL uses the copper wires in your phone line to send internet signals at high speeds, especially if you’re close to the provider’s office.
    
- **Cable**:
    - This is similar to DSL but uses the same coaxial cables that bring TV signals into your home. It can offer faster internet speeds than DSL because it has more bandwidth.
- **Leased Line**:
    - Think of this as renting a private highway for your data. It’s a dedicated connection between two points, between your location and the internet service provider.
- **Metro-optical**:
    - It’s used for connecting buildings within a city or metropolitan area. use light to transmit data very quickly.