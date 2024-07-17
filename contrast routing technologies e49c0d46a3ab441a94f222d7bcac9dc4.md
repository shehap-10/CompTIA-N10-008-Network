# contrast routing technologies

1st: No
2nd: No
3rd: No
Formula: June 27, 2024
Start date: June 26, 2024
Status: 2end
unit/module: 2.2

1. **Routing**:
    - **Definition**: Routing is the process of determining the optimal path for data packets to travel from a source to a destination across a network.
    - **Related Concepts**:
        - **Dynamic Routing**: Dynamic routing protocols allow routers to exchange route information automatically. Examples include:
            - Distance-vector routing protocols (hubs)
                - RIP (Routing Information Protocol),
                - EIGRP (Enhanced Interior Gateway Routing Protocol)
            - Link-state routing protocols (Consider the speed of the link)
                - OSPF (Open Shortest Path First) that builds a global topology database by exchanging link-state advertisements (LSAs) among routers1.
            - Hybrid routing protocols
                - BGP (Border Gateway Protocol)
                    
                    – Determines route based on paths, network policies, or
                    configured rule-sets
                    
                
        - **Static Routing**: Manually configured routes that don’t change dynamically. Useful for specific paths or **default routes.**
        - **Default Route**: A route used when no specific match is found in the routing table.
        - **Administrative Distance**: A value indicating the trustworthiness of a route source (lower values are preferred). Used by the router to determine which routing
        protocol has priority
        - **Exterior vs. Interior Routing**: Exterior routing protocols (like BGP) connect different autonomous systems, while interior routing protocols (like OSPF) operate within a single
            - **Interior routing** stays within the same school (AS) and helps routers communicate within that domain.
            - **Exterior routing** connects different schools (ASes) and enables communication between separate administrative domains.
        - **Time to Live (TTL)**: A field in IP packets that limits their lifetime and prevents infinite loops.
2. **Bandwidth Management**:
    - **Definition**: Managing network resources to optimize bandwidth usage.
    - **Related Concepts**:
        - **Traffic Shaping**: Controlling the flow of traffic to prevent congestion and prioritize certain types of data.
        - **Quality of Service (QoS)**: Techniques to ensure specific traffic (e.g., voice or video) gets higher priority over other traffic.
- [**Enhanced Interior Gateway Routing Protocol (EIGRP)**: A Cisco proprietary protocol that supports multivendor devices and uses a metric based on bandwidth, delay, reliability, and load1](https://community.cisco.com/t5/networking-knowledge-base/dynamic-routing-protocols-ospf-eigrp-ripv2-is-is-bgp/ta-p/4511577).
- **Routing Information Protocol (RIP)**: A simple distance-vector protocol that periodically broadcasts routing tables to neighbors1.
- [**Intermediate System to Intermediate System (IS-IS)**: A link-state protocol similar to OSPF, often used in large service provider networks1](https://community.cisco.com/t5/networking-knowledge-base/dynamic-routing-protocols-ospf-eigrp-ripv2-is-is-bgp/ta-p/4511577).
- [**Border Gateway Protocol (BGP)**: An exterior gateway protocol used for inter-domain routing on the internet1](https://community.cisco.com/t5/networking-knowledge-base/dynamic-routing-protocols-ospf-eigrp-ripv2-is-is-bgp/ta-p/4511577).(explain)