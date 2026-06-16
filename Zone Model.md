Groups reference architecture elements according to defined characteristics. 
The security zone model is developed from the reference architecture. This model is used to describe the logical groupings of assets within an enterprise or a subset of the enterprise.The assets are grouped into entities (e.g., business, facility, site, or IACS). By grouping assets in this manner, a security policy can be defined for all assets that are members of the zone.The model helps to assess common threats, vulnerabilities, and the corresponding countermeasures needed to attain the level of security required for each zone. This analysis can then be used to determine the appropriate protection required based on the activities performed in the zone. Zone policies are independent, and each zone could have totally different security policies.
A security zone is a logical grouping of physical, informational, and application assets sharing common security requirements. The purpose of security zones is to isolate critical components of the system, making it harder for a breach in one part of the network to affect the whole system. A security zone has a border that separates included elements from excluded ones. This border defines what belongs to the zone and how to protect it. This layered security provides defense-in-depth, addressing different levels of security needs. Every situation has a different acceptable level of security. It may not be necessary or practical to apply the same level of security to all components. Security policies are enforced with a combination of measures both at the zone's edge (e.g., firewalls controlling traffic) and inside the zone (e.g., device hardening and malware protection.)
PRINTER ZONE | Simple Example of a Security Zone in an IACS
_What it is:_
A small area in the industrial system where only networked printers are grouped.
_What's inside_:
Industrial report printers (printing alarms, maintenance reports)
Label printers (printing barcode labels for products)
_Why it's a security zone:_
Printers are not critical for controlling machines, but they can be hacked easily.
To protect the important control systems, printers are placed in their own separate zone.
![[Pasted image 20260427152653.png]]
# Conduits
Conduits are secure communication paths that maintain the integrity and confidentiality of data between zones. They can connect two or more zones and may cross a zone to enable flow of information between multiple zones, if security is not compromised. A conduit cannot have subzones. Conduits are either single service (e.g., a single Ethernet network) or consist of multiple data carriers (e.g., network cables, routers, and switches). They can be physical (e.g., cables connecting zones) or logical (e.g., software-defined networks).
![[Pasted image 20260427155223.png]]
## Zone and Conduit Characteristics
**Documenting characteristics of zones and conduits enables:**
- Prioritized security measures and customized solutions
- Risk identification preventing gaps in security and operational oversight
- Quick responses during breaches
- Proper integration, avoids redundancy, and simplifies system maintenance
- Continuous improvement and documentation for auditing
![[Pasted image 20260427155343.png]]

This is a **SCADA zone and conduit example**.
A wide area network, WAN is located in the middle. The conduits are highlighted in red. There are public-private telephone networks and radio microwaves. The zones include a primary control center and a backup control center, with similar equipment on both sides. And then, there are control zones for Sites A, C, X, and Z. Zone and conduit models can help us start thing about security. We started asking ourselves questions like, does that make sense? Is it cost-effective from a security perspective? What am I protecting? Is there a way for an attacker to get in?
![[Pasted image 20260427155420.png]]
