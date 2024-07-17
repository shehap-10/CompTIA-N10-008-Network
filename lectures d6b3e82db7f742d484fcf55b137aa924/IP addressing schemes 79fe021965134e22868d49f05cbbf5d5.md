# IP addressing schemes.

1st: Yes
2nd: No
3rd: No
Formula: June 26, 2024
Start date: June 21, 2024
Status: 2end
unit/module: 1.4

- how many octet do we have in ipv4 `4` each one of them 8 bits
    
    
- how do hosts know which portion of the 32-bits identifies the network and which identifies the host?
    
    That is the role of the subnet mask.
    
    ![Untitled](IP%20addressing%20schemes%2079fe021965134e22868d49f05cbbf5d5/Untitled.png)
    
- what is the using of subnet mask
    
    This is used to identify the network/host portion of the IPv4 address.
    
    Note that the subnet mask does not actually contain the network or host portion of an IPv4 address, it just tells the computer where to look for the part of the IPv4 address that is the network portion and which part is the host portion.
    
- The actual process used to identify the network portion and host portion is called `ANDing.`
    
    ![Untitled](IP%20addressing%20schemes%2079fe021965134e22868d49f05cbbf5d5/Untitled%201.png)
    
    refers to the process of performing a bitwise AND operation on IP addresses and subnet masks to determine the network address.
    
- what network address how to find it?
    
    • **Network address (192.168.10.0)** - The logical AND operation between the IPv4 address and subnet mask results in an IPv4 network address shown in dotted decimal and binary formats.
    
- what is the ipv4 it never be assigned host addresses
    
    network address (lowest host number)
    
    broadcast address (highest host number)
    
    ![Untitled](IP%20addressing%20schemes%2079fe021965134e22868d49f05cbbf5d5/Untitled%202.png)
    
- what is The difference between unicast Broadcast multicast
    
    Unicast transmission refers to one device sending a message to one other device in one-to-one communications.
    
- The difference between public IP private IP ?
    
    ## private
    
    NOT organized by over the Internet assigned by admin unique in LAN
    
    should start with on of the class 
    
    # The Private Address
    
    | Network Address and Prefix | RFC 1918 Private Address Range |
    | --- | --- |
    | 10.0.0.0/8 (A) | 10.0.0.0 - 10.255.255.255 |
    | 172.16.0.0/12 (B) | 172.16.0.0 - 172.31.255.255 |
    | 192.168.0.0/16 (C) | 192.168.0.0 - 192.168.255.255 |
    
    ### public
    
    organized by over the Internet assigned by [IANA](service provid) unique in Global routed  between Internet service provider (ISP)
    
    ## **Summary of IPv4 Classes**
    
    | Type | Public IP Range | Private IP Range | Subnet Mask | # of Networks | # of Hosts per Network |
    | --- | --- | --- | --- | --- | --- |
    | Class A | 1.0.0.0 to127.0.0.0 | 10.0.0.0 to10.255.255.255 | 255.0.0.0 | 126 | 16,777,214 |
    | Class B | 128.0.0.0 to191.255.0.0 | 172.16.0.0 to172.31.255.255 | 255.255.0.0 | 16,382 | 65,534 |
    | Class C | 192.0.0.0 to223.255.255.0 | 192.168.0.0 to192.168.255.255 | 255.255.255.0 | 2,097,150 | 254 |
- what is the type of IP
    
    ![Untitled](IP%20addressing%20schemes%2079fe021965134e22868d49f05cbbf5d5/Untitled%203.png)
    
- what is Loopback  &  Link-local address  addresses what rang of IP
    - 127.0.0.1-127.255.255.254 this is the rang of loopback used on a host to test if TCP/IP is operational
    - 169.254.0.1-169.254.255.254 Known as automatic private IP address or self assign address (Link-local address) used by DHCP to Self configure the device when no  DHCP service are available
    - APIPA
        
        APIPA (Automatic Private IP Addressing) is a feature in Windows-based operating systems that allows a device to automatically assign itself an IP address when it is unable to obtain one from a DHCP server. The IP address range for APIPA is 169.254.0.1 to 169.254.255.254, with a subnet mask of 255.255.0.0.
        
- What's the reason for using subnetting
    - reduce the size of the network why? improve the performance I reduce the traffic on the network
    - Implementing secure policy between subnetting
    - Some type of organization like location groups and type of devices
- `DMZ` it is the servers side Public IP of the of the company that provides service to the Internet
- how the subnetting work
    
    ![Untitled](IP%20addressing%20schemes%2079fe021965134e22868d49f05cbbf5d5/Untitled%204.png)
    
    ![Untitled](IP%20addressing%20schemes%2079fe021965134e22868d49f05cbbf5d5/Untitled%205.png)
    
    ![Untitled](IP%20addressing%20schemes%2079fe021965134e22868d49f05cbbf5d5/Untitled%206.png)
    
    ![Untitled](IP%20addressing%20schemes%2079fe021965134e22868d49f05cbbf5d5/Untitled%207.png)
    
    - to To figure out how many hosts will be in the network (n=how many Zero in the IP)
    
    $$
    2^n-2
    $$
    
    Number of subnet Bits = how many the Subnet mask borrow from the host
    
    ![Untitled](IP%20addressing%20schemes%2079fe021965134e22868d49f05cbbf5d5/Untitled%208.png)
    
    Number of subnets created= (X=How many one in the last octet subnet mask)
    
    $$
    2^x
    $$
    
    broadcast address on this subnet =1-binary 2- set the host bits to ones 1(Any zeros in the subnet mask turn the IP into one)
    
    [](https://www.youtube.com/watch?v=79u-4KfaWYE)
    
- what is VLSM
    
    It's when you submit the subnet mask
    

[](https://www.youtube.com/watch?v=Knv6Y1R2OPg)