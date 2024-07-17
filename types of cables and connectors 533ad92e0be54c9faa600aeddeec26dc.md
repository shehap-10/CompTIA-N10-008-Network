# types of cables and connectors

1st: Yes
2nd: No
3rd: No
Formula: June 25, 2024
Start date: June 20, 2024
Status: 2end
unit/module: 1.3

- `bandwidth` is who much capacity can medium can carry data
    
    It's measure how many bits can transform in second
    
    $$
    bps = 1bps < kpps=10^3 <Mbps = 10^6 < Gbps =10^9 < Tbps = 10^12
    $$
    
- `latency` is the mount of time including delays for data to travel
    
    
- `Throughput` is a measure of how much data can be transferred within a specific time frame
- `Goodput` is the measure of useful data transferred over a network
    
    ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled.png)
    
- **Types** of copper cabling
    
    ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled%201.png)
    
- what it the benefit form twisted pairs in copper cabling
    
    protect the signal interferences and isolates the wires from each other 
    
- what  kind of  caused Signal EMI/RFI
    
    EMI typically involves interference caused by electromagnetic radiation, while RFI specifically refers to interference caused by radio-frequency signals. Both can lead to performance issues and signal degradation in electronic equipment.
    
- STP vs UTP copper
    
    ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled%202.png)
    
    ### STP
    
    Better noise protection more expensive harder to install he had EMI/RFI protection
    
- What is the purpose of using two wires with equal and opposite signals in twisted pair cabling?
    
    one positive (Transmit+ or Receive+) and one negative (Transmit- or Receive-). If one wire is +1V, the other is -1V simultaneously.
    
- coaxial cables vs twinaxial cable
    
    cable modem
    
    tow inner conductors
    
    full duplex 
    
    five meters
    
- what are different **types** connectors used with coax cable
    
    BNS
    
    F-type
    
    RG-6
    
    ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled%203.png)
    
- straight-through vs Crossover cable (old) before `Auto-MDix`
    
    Straight through different devices like host to switch or switch to a router. both ends should be the same T568B or T568A (T568B Used now days)
    
    crossover from the same devices switch to switch or router to router. One end T568A other end T568B
    
    rollover cable = used to connect workstation to switch Through console port 
    
- what Features and types of fiber-optic cabling have ?
    
    transmit data over long distance and high bandwidth in any network media. flexible. extremely thin made pure glass Use laser or led to encode bits not affected by electrical noises. Minimum signal loss. not affected by EMI/RFI  
    
    ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled%204.png)
    
    use of fiber within the ,enterprise ,home ,long networks , submarine
    
    cladding it’s not reflected like the core 
    
- what type of fiber-optic connectors
    
    ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled%205.png)
    
    1. Subscriber Connector
        1. features a push-pull mechanism that is commonly used with multimode fiber?
- `half-duplex` is a communication mode in which data can be transmitted in one way only
- what is the type of wireless standards
    
    ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled%206.png)
    
- `Auto-MDix`
- T568A (أخضر) vs T568B (**ب**رتقالي)
    
    many organizations use T568B standard for all the networks 
    
    ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled%207.png)
    
     "C:\Users\pc\Videos\2024-06-12 16-49-55.mkv”
    
- what is it RJ11 ? how many positions ? what is use for ?
    - "Registered Jack 11". It is a standardized telecommunication network interface for connecting voice and data equipment.
    - RJ11 connectors have six positions, but often only two or four of these positions are used.
    - used for
        - **Telephone Lines**:
        - **DSL Connections**:
            - For Digital Subscriber Line (DSL) internet services, RJ11 connectors are used to connect the DSL modem to the telephone line.
- Angled physical contact (APC) vs Ultra-physical contact (UPC)
    - A
        
         connector end-face finish where the fiber end is polished at an angle, around 8 degrees.
        
        The angled polish reduces the amount of reflected light from the connector end-face.
        
        such as in high-speed data transmission, long-distance telecommunications, and fiber-to-the-home (FTTH) networks
        
    - U
        
        type of fiber optic connector end-face finish where the fiber end is polished flat.UPC connectors have a higher level of back reflection compared to APC
        
        where moderate return loss is acceptable.
        
- Transceivers/media converters
    - media converters
        
        ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled%208.png)
        
    - Transceiver
        
        ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled%209.png)
        
        - types
            
            
            | Feature | SFP | SFP+ | QSFP | QSFP+ |
            | --- | --- | --- | --- | --- |
            
            | Data Rate | Up to 1 Gbps | Up to 10 Gbps | Up to 40 Gbps | Up to 100 Gbps |
            | --- | --- | --- | --- | --- |
            
            | Number of Channels | Single | Single | Four | Four |
            | --- | --- | --- | --- | --- |
            
            | Typical Use | Low to Medium Speed | Medium to High Speed | High Speed | Ultra High Speed |
            | --- | --- | --- | --- | --- |
            
            | Application | Networking, Telecom | Data Centers | Data Centers, High-Speed | Data Centers, High-Speed |
            | --- | --- | --- | --- | --- |
            
            the number of channels indicates how many separate data pathways the transceiver module can support simultaneously. 
            

### Cable management

- Patch panel/patch bay
    
    C:\Users\pc\Videos\2024-06-12 20-06-42.mkv
    
    patch panel as the main control center of the building’s network.
    
    ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled%2010.png)
    
- **Punchdown Block**
- Fiber distribution panel
    
    ![Untitled](types%20of%20cables%20and%20connectors%20533ad92e0be54c9faa600aeddeec26dc/Untitled%2011.png)
    

The 802 standards, developed by the IEEE (Institute of Electrical and Electronics Engineers), are a family of standards primarily concerned with local area networks (LAN) and metropolitan area networks (MAN). Here are some of the key 802 standards:

- **IEEE 802.3**: Ethernet - Specifies the physical layer and media access control (MAC) for wired Ethernet networks.
- **IEEE 802.11**: Wi-Fi - Specifies the protocols for wireless local area networks (WLANs), commonly known as Wi-Fi.
- **IEEE 802.15**: Wireless Personal Area Networks (WPANs) - Includes standards such as Bluetooth (802.15.1) and Zigbee (802.15.4).
- **IEEE 802.16**: Broadband Wireless Access (BWA) - Commonly known as WiMAX, it specifies standards for wireless metropolitan area networks (WMANs).
- **IEEE 802.1**: Bridging and Network Management - Deals with network management and internetworking, including standards like 802.1Q for VLANs (Virtual Local Area Networks).
- **IEEE 802.2**: Logical Link Control (LLC) - Provides specifications for the data link layer in the OSI model.

These are some of the essential 802 standards, each addressing different aspects of networking and communication.