**Network security technologies, including** network security devices, network architecture, and intrusion detection systems****, work together to form a multi-layered defense strategy that helps organizations prevent and detect security incidents.
When configured appropriately, these technologies **govern what traffic can or cannot move through the network**, either actively blocking via firewalls or data diodes or passively detecting via IDS.
# Network Security Devices
**Hardware/software that controls and monitors network traffic to protect against unauthorized access or attack**
- **Firewalls**
    - Act as **gatekeepers** between network segments, **inspecting and filtering traffic based on rules** 
    - Used to enforce **boundaries** between zones (e.g., Control Zone and Enterprise Zone)
    - Help prevent unauthorized access and reduce the risk of cyberattacks

- **Unidirectional gateways (data diodes)**
    - Hardware-enforced **one-way communication** devices
    - **Allow data to flow out** of the control system (e.g., to monitoring systems or historians) but **block all inbound traffic**
    - Provide strong protection for critical systems by physically preventing external access
# Network Architecture
**The structured design of a network, including how systems are segmented, secured, and connected**
- **Defined zones**
    - Networks are divided into zones (e.g., Control, DMZ, Enterprise) to **contain and control traffic flow**
    - Minimizes the "blast radius" if a compromise occurs
    - Supports least privilege and **defense-in-depth** principles
- **Demilitarized Zone (DMZ)**
    - A **buffer zone** between trusted internal networks and less-trusted external ones
    - Used to host systems like remote access, data aggregation servers, and patch repositories in a more controlled space
# Intrusion Detection Systems
**Security tools that monitor network or device activity for signs of malicious behavior**
- **Network-based IDS (NIDS)**
    - **Monitors traffic** on the network for suspicious activity or known attack signatures
    - **Non-intrusive** — does not block traffic, only alerts on anomalies
    - Can detect lateral movement, scanning, or unauthorized communications
- **Host-based IDS (HIDS)**
    - **Installed on individual devices** (e.g., engineering workstations, servers)
    - **Monitors local behavior** such as file changes, process activity, or configuration modifications
    - Provides visibility into potential threats targeting specific assets
# Firewalls
## Firewall Overview
- **A firewall is a device that regulates and restricts data communication between two connected networks.** It **filters and monitors network traffic** based on predefined **rules**.
- Firewalls can be implemented as **software** on a general-purpose computer or deployed as dedicated **hardware appliances**.
- They **inspect, forward, or block** network packets according to configured **policies**.
- Firewalls are commonly used to **define and enforce boundaries** between different network zones.
- The **rules** set in a firewall typically control which ports and protocols are **allowed or blocked**.
## Hardware Firewalls
A **hardware firewall** is a dedicated physical device that protects a network by **monitoring and filtering incoming and outgoing traffic** between internal systems (like industrial networks) and external networks (like the internet).
 The firewall acts as a **gateway for all traffic**, which is then evaluated against a **set of rules or polices** that determine if the traffic **allowed or denied**.
Unlike a software firewall that runs on a computer, a hardware firewall is an **appliance placed at the network perimeter** to protect PLCs, SCADA systems, and similar infrastructure from external threats and unauthorized access.

- ## Classes of Firewalls
### Packet Filter:
**Inspects and filters individual network packets based on simple criteria like IP address, port, and protocol**
- Examines only the headers of each packet of information (source, destination, function, port)
- Accepts or rejects based on Access Control Lists (ACLs)
- Administrators can create their ACLs based on Address, Protocols and Packet attributes
- Pros: Fast and cheap
- Cons: only looks at header info
### **Stateful Inspection:**
**Tracks active connections and filters traffic based on the context of ongoing communication sessions**
- Tracking the relationships between packets in a session
- Inspecting the packet’s structure and sequence
- Can be either hardware-based (e.g. Cisco ASA, Tofino) or server-based (e.g. CheckPoint Firewall-1)
- Pros:  Relatively Fast, Flexible, Improved Security
- Cons:  Can be spoofed by attacker after establishing a connection
### **Application Proxy:**
**Acts as an intermediary between devices, terminating and re-establishing connections to inspect traffic at the application level**
- Can inspect application data (like HTTP requests or FTP commands)
- Pros: Strong filtering  
- Cons: Slower due to deep analysis
### **Deep Packet Inspection (DPI):**
**Examines the full contents of network packets, including payloads, to detect protocol-specific commands or malicious content**
- Open up the packet and examine the data inside (application commands, files, or even text).
- They can identify specific applications, malware signatures, or policy violations—even if the traffic is using standard ports.
- Pros: Offers advanced protection  
- Cons: Complex and requires more resources
## Firewall Policy
Installing a firewall is usually simple, but its true security value lies in **proper configuration** — a more complex process that requires deep technical knowledge and a strong understanding of the network.
**Its effectiveness depends heavily on the quality of its rules and policies**, which must be thoughtfully designed, continuously reviewed and regularly updated.

## IACS Firewalls
Many companies offer **purpose-built firewalls designed explicitly for IACS environments.**
They are used to secure vulnerable devices such as **PLCs, RTUs, and DCS controllers**, which often lack native security features.
**Key features of IACS-specific firewalls:**
- **Industrial form factor and robustness:** Designed to withstand harsh environments (dust vibrations, extreme temperatures, etc.) found in control panels or field installations
- **Electrician / Control Tech friendly:** Often DIN-rail mountable, easy to wire and offer simple interfaces, reducing reliance on IT support
- **Knowledge of industrial protocols:**  Supports deep packet inspection (DPI) for ICS protocols like Modbus, DNP3, etc. allowing the firewall to filter traffic based on command type, not just port or IP address
- **Extensibility beyond just packet filtering:** Offer advanced security features such as logging and alerts, intrusion detection, fail safe behavior, zone based segmentation etc.
![[Pasted image 20260428123029.png]]
![[Pasted image 20260428123053.png]]
## **Unidirectional Gateway**
A **unidirectional gateway** is a hardware-enforced (not dependent on software configuration or patching) network device (often called a **data diode**) that **allows data to travel only in one direction**—from a source network to a destination network with no physical path for return traffic
Normal flow control SYN ,SYN-ACK, ACK requires two-way handshaking, so it must be emulated to allow one-way protocols to function.
Commonly used in defense and nuclear power plants, **unidirectional gateways are increasingly used in IACS** to prevent external access to critical infrastructure and allow real-time visibility from a secure OT network into IT systems without risk of remote intrusion.