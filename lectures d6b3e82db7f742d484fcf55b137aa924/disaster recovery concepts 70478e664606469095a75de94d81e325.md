# disaster recovery concepts

1st: No
2nd: No
3rd: No
Status: 2end

- **Multipathing**: .
    - Using multiple network paths to enhance reliability allowing data to reroute through alternative paths if one path fails.
- **NIC Teaming**:
    
    involves grouping physical network adapters to enhance performance and redundancy by enabling load balancing and failover capabilities through a single IP address across multiple physical connections, 
    
    network interface card (NIC) teaming, also known as bonding, balancing, or aggregation
    
- **Redundant Hardware/Clusters**:
    
    Redundant hardware ensures continuous operation by replacing failed components automatically. This applies to devices like switches, routers, and firewalls. Clustering, on the other hand, balances loads and provides fault tolerance by distributing tasks across multiple servers. It enhances redundancy, reliability, and scalability.
    
    Server clustering protects against outages caused by software failures, hardware malfunctions (like overheating or component failures), and external events such as power disruptions or natural disasters. These clusters are designed to handle various types of failures to ensure uninterrupted service.
    

### Facilities and infrastructure support

- Uninterruptible power supply (UPS)
    
    UPS devices provide backup power during electrical outages or fluctuations.
    
    - They ensure continuous power supply to critical systems, allowing time for graceful shutdown or failover Timperley
- Power distribution units (PDUs)
    - **Role**: PDUs distribute power from UPS or other sources to various devices. توصيله
- Generator
    
    Generators act as backup power sources when UPS batteries are depleted ماطور
    
- HVAC
    
     HVAC systems regulate temperature and humidity in data centers.
    
- Fire suppression
    
    Fire suppression systems protect against fires that could damage equipment.
    
- RTO vs RPO
    - **Recovery Time Objective (RTO)**:
        - **Definition**: RTO represents the maximum acceptable downtime for a system or application after a failure occurs.
    - **Recovery Point Objective (RPO)**:
        - **Definition**: RPO defines the maximum data loss acceptable during recovery.
- MTTR vs MTBF
    - **Mean Time to Repair (MTTR)**:
        - **Focus**: It measures how quickly you can restore functionality after a failure occurs.
        - **Definition**: MTTR represents the average time it takes to repair a failed system or component.
        - **Example**: If a server fails and it takes 2 hours to diagnose, 4 hours to fix, and 1 hour for testing, the MTTR is 7 hours.
    - **Mean Time Between Failures (MTBF)**:
        - **Definition**: MTBF represents the average time between consecutive failures of a system or component.
        - **Focus**: It quantifies reliability by measuring the system’s stability over time.
- **Active-Active vs. Active-Passive**:
    
    Active-active systems share the load, while active-passive systems have a standby backup.
    
- **Cold Site**: A backup location with minimal infrastructure, suitable for non-critical applications.
- **Warm Site**: A partially equipped backup site with some infrastructure.
- **Hot Site**: A fully operational backup site with real-time data synchronization.

**Virtual Router Redundancy Protocol (VRRP)**:

- **Objective**: VRRP also provides gateway redundancy, but it’s not tied to any specific vendor (unlike Cisco’s HSRP).

**First Hop Redundancy Protocol (FHRP)**:

- **Purpose**: FHRP ensures that if your main gateway router fails, there’s a backup ready to take over without disrupting network connectivity.