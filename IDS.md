**Intrusion Detection Systems (IDS)** are tools that **monitor and analyze network or system activity** for signs of unauthorized access, misuse, or abnormal behavior.
They act like a “burglar alarm” for your network, generating **alerts so administrators can take action** if a threat is detected. They inspect log-ins, network traffic, and system events in real time or near real time.
An **IDS complements other preventive tools** like firewalls and access control systems, helping to build a defense-in-depth strategy.
Intrusion detection systems **can be configured** to monitor traffic between PLCs, HMIs, SCADA, and other legacy devices.
Common **ICS-specific platforms** (Nozomi, Claroty, Dragos) understand industrial protocols and baseline “normal” behavior to detect anomalies.
### Types of IDS
#### Network Intrusion Detection Systems - NIDS
- Monitor traffic between devices
- Uses pre-defined rules (signature-based) to flag malicious activity
- Detects behavior (heuristics-based) that deviates from established norms
- Incorporates passive sniffing to monitor traffic without affecting flow or adding latency
#### Host Intrusion Detection System - HIDS
- Tracks internal activity (file access, user logins, config changes)
- Uses pre-defined rules (singature-based) to look for patterns that match known attack signatures.
- Detects unusual behavior (heuristics-based) or changes to critical files, user privileges, or process activity
- Uses a software agent installed directly on the host, collecting data and sending alerts to a centralized system 
### IDS Challenges and Limitations
1. False positives
2. Deployment and operational costs
3. Limited signatures for control system protocols (legacy devices)
4. Requires continuous care and feeding