# network services

1st: Yes
2nd: No
3rd: No
Formula: June 28, 2024
Start date: June 23, 2024
Status: Hard
unit/module: 1.6

### **DHCP (Dynamic Host Configuration Protocol)**

- **What is Scope?**
    
    A DHCP scope defines a range of IP addresses that the DHCP server can lease (renting) to clients within a specific subnet. It ensures efficient IP address management.
    
- **what is Exclusion Ranges?**
    
     These are specific IP addresses within the scope that the DHCP server avoids leasing. For example, you might exclude addresses for network infrastructure devices ( **for devices that require static IPs, such as servers, printers**)
    
- **Reservation**:
    
     DHCP reservations assign specific IP addresses to particular devices based on their MAC addresses. This ensures consistent IP assignments ensure that critical devices (like servers, printers, or network infrastructure) always receive the same IP address.
    
- dynamic assigned vs static assigned
    
    **dynamic**  automatic allocation of IP addresses from the DHCP **for a specific lease duration**
    
     **Static** assignment means manually configuring a device with a fixed IP address rather than using DHCP [**Reservation**:](network%20services%203208ca38085e4e65b290ce54d3f89752.md) (Other names - Static DHCP Assignment, Static DHCP, Address Reservation, IP Reservation) 
    
- **Lease Time**:
    
    The duration for which a client holds an assigned IP address. After the lease expires, the client must renew it. 
    
    - DHCP renewal
        - T1 timer to renew the IP address 50% of the lease time (by default)
        - T2 timer
            - If the original DHCP server is down try rebinding with any DHCP server 87.5% of the lease time
- Scope options:
    
    are additional configuration settings provided by DHCP, such as default gateway, DNS servers, domain name, etc.
    
- **Available Leases**:
    
    The number of unassigned IP addresses in the DHCP pool.
    
- DHCP Relay
    - DHCP relay is a service that forwards DHCP requests from clients in subnets without a local DHCP server to a DHCP server on another subnet.
    - Typically configured on routers or switches using the IP helper address command.
        
        [127133.avif](network%20services%203208ca38085e4e65b290ce54d3f89752/127133.avif)
        
- IP Helper/UDP Forwarding
    
    refers to the process of forwarding DHCP (and other) broadcast traffic to a specific IP address.
    
    commonly used in conjunction with DHCP relay to ensure that DHCP requests reach the DHCP server.
    

### NTP (Network Time Protocol)

- Stratum
    - Stratum levels indicate the distance from the reference clock in the NTP hierarchy.
    - NTP servers are organized into strata (levels). Stratum 0 includes highly accurate clocks (e.g., atomic clocks), and each subsequent level (Stratum 1, 2, etc.) syncs with the one above.
- **Clients**:
    
    Devices that synchronize their clocks using NTP.
    
- **Servers**:
    
     Provide accurate time information to clients.
    

## DNS (Domain Name System)

1. **Record Types**:
    1. **A Record**: Maps domain names to IPv4 addresses.
    2. **AAAA Record**: Maps domain names to IPv6 addresses.
    3. **CNAME (Canonical Name)**: Creates an alias for a domain name.
    4. **MX (Mail Exchange)**: Specifies mail server addresses for email delivery.
    5. **SOA (Start of Authority)**: Contains administrative information about a domain.
    6. **PTR (Pointer)**: Resolves IP addresses to domain names (reverse DNS).
    7. **TXT (Text)**: Holds arbitrary text information.
    8. **SRV (Service)**: Defines services available on a domain.
    9. **NS (Name Server)**: Lists authoritative DNS servers for a domain.
2. **Global Hierarchy**: DNS operates in a hierarchical structure, with root servers at the top.
3. **Root DNS Servers**: The initial point of DNS resolution.
4. **Internal vs. External DNS**: Internal DNS resolves local domain names, while external DNS handles public domains.
5. **Zone Transfers**: Synchronize DNS data between primary and secondary servers.
6. **Authoritative Name Servers**: Hold DNS records for specific domains.
7. **Time to Live (TTL)**: Specifies how long DNS records can be cached.
8. **DNS Caching**: Improves performance by storing resolved queries.
9. **Reverse DNS/Reverse Lookup/Forward Lookup**: Reverse DNS maps IP addresses to domain names.
10. **Recursive Lookup/Iterative Lookup**: Recursive DNS servers perform full lookups, while iterative servers provide partial answers.

### DNS (Domain Name System)

### Record Types

- **Definition**: DNS record types are different kinds of data stored in a DNS database, each serving a specific purpose in the domain name resolution process.
- **Common Types**: Include A, AAAA, CNAME, MX, SOA, PTR, TXT, SRV, and NS records.

### Address (A vs. AAAA)

- **A Record**: Maps a domain name to an IPv4 address.
- **AAAA Record**: Maps a domain name to an IPv6 address.

### Canonical Name (CNAME)

- **Definition**: A CNAME record maps an alias name to a true or canonical domain name.
- **Use Case**: Allows multiple domain names to map to a single IP address without managing separate A/AAAA records for each alias.

### Mail Exchange (MX)

- **Definition**: MX records specify the mail servers responsible for receiving email on behalf of a domain.
- **Priority**: MX records have a priority value to determine the order in which mail servers should be used.

### Start of Authority (SOA)

- **Definition**: The SOA record provides essential information about a DNS zone, including the primary name server, the email of the domain administrator, and various timers.
- **Components**: Include serial number, refresh interval, retry interval, expire time, and minimum TTL.

### Pointer (PTR)

- **Definition**: PTR records map an IP address to a domain name, used primarily for reverse DNS lookups.
- **Purpose**: Verifies the domain name associated with an IP address.

### Text (TXT)

- **Definition**: TXT records allow domain administrators to insert arbitrary text into a DNS record.
- **Use Case**: Commonly used for verification purposes, such as domain ownership verification, and to implement security policies like SPF (Sender Policy Framework).

### Service (SRV)

- **Definition**: SRV records specify the location of servers for specific services.
- **Use Case**: Used in VoIP and other applications to define the hostname and port number for services like SIP.

### Name Server (NS)

- **Definition**: NS records specify the authoritative name servers for a domain.
- **Purpose**: Ensure that DNS queries for the domain are directed to the correct servers.

### Global Hierarchy

- **Structure**: DNS is organized hierarchically, starting from the root level down to TLDs (top-level domains) and further to individual domain names.
- **Components**: Include root DNS servers, TLD servers, and authoritative DNS servers.

### Root DNS Servers

- **Definition**: The root DNS servers are the highest level in the DNS hierarchy and contain information about top-level domains (TLDs).
- **Function**: They direct queries to the appropriate TLD servers.

### Internal vs. External

- **Internal DNS**: Used within an organization's private network to resolve internal domain names.
- **External DNS**: Used to resolve public domain names on the internet.

### Zone Transfers

- **Definition**: Zone transfers are the process of replicating DNS databases across multiple DNS servers.
- **Types**: Include full zone transfers (AXFR) and incremental zone transfers (IXFR).

### Authoritative Name Servers

- **Definition**: Authoritative name servers provide answers to DNS queries from their own data, rather than relying on data from other servers.
- **Purpose**: Ensure accurate and reliable DNS resolution for a specific domain.

### DNS Caching

- **Definition**: DNS caching stores DNS query results temporarily to improve response times and reduce the load on DNS servers.
- **Implementation**: Done by both client resolvers and intermediate DNS servers.

### Reverse DNS/Reverse Lookup/Forward Lookup

- **Reverse DNS**: Resolves an IP address to a domain name using PTR records.
- **Forward Lookup**: Resolves a domain name to an IP address using A or AAAA records.

### Recursive Lookup/Iterative Lookup

- **Recursive Lookup**: The DNS resolver queries multiple DNS servers on behalf of the client to resolve a domain name.
- **Iterative Lookup**: The DNS resolver queries each DNS server one at a time, returning the best answer it can until it finds the final answer.