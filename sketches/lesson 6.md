# **Plan for Lesson 6 Cheat Sheet: Data Communication & Networking**

### **The Goal**

To create a comprehensive, single-page reference sheet covering all core concepts of data communication and networking from the syllabus, with a special focus on details relevant for MCQ questions.

### **The Structure: "From Physical Signals to Secure Applications"**

The cheat sheet will be structured into four logical sections that follow the layered approach of networking, making it easy to understand how different technologies fit together.

## **Final Content List for the Cheat Sheet**

### **Part 1: Physical Layer Concepts (Signals & Media)**

* **Data Communication Model:** Sender → Message → Medium → Receiver → Protocol.  
* **Signal Types:** Analog (continuous wave) vs. Digital (discrete steps).  
* **Signal Properties:**  
  * Amplitude, Frequency, Wavelength, Phase.  
* **Transmission Media:**  
  * **Guided:** Twisted Pair, Coaxial Cable, Fiber Optic.  
  * **Unguided:** Radio Waves, Microwaves.  
* **Signal Impairment (How signals get corrupted):**  
  * Latency: Delay in data travel.  
  * Bandwidth: Frequency range a medium can carry.  
  * Noise: Unwanted signal interference.  
  * Attenuation: Loss of signal strength over distance.  
  * Distortion: Change in the signal's shape.  
* **Modulation & Encoding:**  
  * **Analog Modulation:** AM, FM, PM.  
  * **Digital-to-Analog:** ASK, FSK, PSK.  
  * **Digital Encoding:** Manchester encoding (aids synchronization).

### **Part 2: Data Link Layer Concepts (LANs & Access)**

* **Network Topologies:** Bus, Star, Ring, Mesh (with simple diagrams).  
* **Networking Hardware:**  
  * NIC (Network Interface Card): Connects a device to the network.  
  * Hub: Broadcasts data to all (Dumb).  
  * Switch: Sends data to the intended port (Intelligent).  
  * Bridge: Connects two similar LANs.  
* **MAC (Media Access Control):**  
  * MAC Address: 48-bit unique hardware address of a NIC.  
  * Frame: The unit of data at the Data Link layer, containing MAC addresses.  
* **Media Access Control Protocols:**  
  * Purpose: To manage orderly access to a shared medium.  
  * Evolution: ALOHA → Ethernet (CSMA/CD).  
* **Error Control:**  
  * Parity Check: Adding a parity bit to detect single-bit errors.

### **Part 3: Network & Transport Layer Concepts (Internetworking)**

* **IP Addressing:**  
  * **Versions:** IPv4 (32-bit) vs. IPv6 (128-bit).  
  * **IPv4 Classes:** A, B, C (with their first octet ranges).  
  * **Private IP Ranges:** e.g., 192.168.x.x, 10.x.x.x.  
  * **Subnetting:** Dividing a large network into smaller sub-networks.  
  * CIDR notation (e.g., /24).  
* **Routing & Internetworking Hardware:**  
  * Router: Connects different networks, finds the best path for data packets.  
  * Gateway: Connects networks using different protocols.  
* **Core Internet Concepts:**  
  * Packet Switching: Breaking messages into smaller packets that travel independently.  
  * Best-effort delivery: The network doesn't guarantee packet delivery.  
* **Transport Layer Protocols:**  
  * **Ports & Multiplexing:** How multiple applications use the network at once.  
  * UDP (User Datagram Protocol): Connectionless, no delivery guarantee (Fast; used for DNS, streaming).  
  * TCP (Transmission Control Protocol): Reliable, connection-oriented, ordered delivery (slower; used for web, email).

### **Part 4: Application, Security & Connectivity**

* **Reference Models:**  
  * OSI Model (7 Layers): A conceptual framework (Physical, Data Link, Network, Transport, Session, Presentation, Application).  
  * TCP/IP Model (4 Layers): The practical model used on the internet.  
* **Application Layer Services:**  
  * DHCP (Dynamic Host Configuration Protocol): Automatically assigns IP addresses.  
  * DNS (Domain Name System): Translates domain names to IP addresses.  
  * NAT (Network Address Translation) & Proxy Server: Allows devices with private IPs to access the internet.  
* **Connectivity:**  
  * ISP (Internet Service Provider): Provides internet access.  
  * DSL/ADSL: Broadband technology over telephone lines.  
  * Modem (Modulator/Demodulator): Converts signals for transmission over different media (e.g., PSTN).  
* **Network Security:**  
  * **Encryption:** Symmetric (one key) vs. Asymmetric (public/private keys).  
  * **Digital Signature:** Authenticates the sender and message integrity.  
  * **Threats:** Viruses, Trojans, Malware, Phishing.  
  * **Protection:** Firewalls, Antivirus software.