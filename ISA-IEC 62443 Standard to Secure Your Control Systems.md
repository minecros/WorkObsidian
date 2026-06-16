# 1. Introduction to control system security
## Defining Control System Security
Control system cybersecurity is the protection of the computer systems and networks that manage and automate industrial processes
**Electronic Security:** Actions required to protect critical systems or informational assets from unauthorized use, denial of service, modifications, disclosure, loss of revenue, or destruction.
**Control System:** Hardware and software components of an Industrial Automation and Control System ([[IACS]]).
**Cybersecurity** is defined as measures taken to protect a computer or computer system against unauthorized access or attack.
**Control System Cybersecurity** is the protection of the computer systems and networks that manage and automate industrial processes.
## Trends in Control System
Why control system cybersecurity matters more than ever?
- Increase in Attempts and Attacks
- More [[COTS]] - Modern control systems now rely heavily on COTS that are mass-produced, readily available, and easy to install. While this makes deployment faster and cheaper, it introduces risk. 
- Internet Protocols Expose Control Systems - industrial control systems increasingly use the standard TCP/IP communication protocols, just like business IT systems. This has made integration easier. However, it also means the control system has inherited all the same network vulnerabilities found in traditional IT. 
- Difficult to Separate IT and OT Networks - maintaining a strict separation between business and operational networks is becoming increasingly difficult. In many environments, particularly those with legacy systems, full isolation is not practical or even possible.
- Remote Access - These technologies have become essential for maintenance and efficiency, but they may also increase the attack surface.
- Automated Attacks - today, even attackers with limited technical skills can launch attack using automated tools.
- Published [[IACS]] Vulnerabilities 
### Potential consequences for organizations
- Unauthorized access, theft, or misuse data
- Loss of integrity or reliability of the control system
- Loss of control system availability and/or other operational disruption
- Equipment and/or reputational damage
- Personal injury
- Financial losses and/or loss of competitive advantage
- Violation of legal and regulatory requirements
- Decreased employee morale
### Potential consequences for society
- Economic and political instability
- Social unrest
- Threats to national security
- Psychological or physical harm
- Erosion of trust in the system
- Privacy concerns including loss of personal data
- Disruption of critical services
- Intellectual Property theft
## Cybersecurity Concepts
### Defense-in-depth
Defense-in-depth is a security strategy that applies multiple layers of protection across different levels of a system to prevent cyber threats and minimize damage if an attack occurs.
A perimeter defense is **NOT** enough. The bad guys will eventually get in. Rather than relying on a single point of defense, it **creates redundant and complementary protections** across the entire system.
This approach ensures that:
- Attackers must bypass or break through **multiple, independent layers, increasing the chances of detection.**
- A vulnerability in one layer can be mitigated by the strengths of another, reducing overall risk.
- **Security becomes layered** not only across the network, but also within individual systems, making compromise more difficult and costly for adversaries.
### Detection in depth
 Detection-in-depth is the strategy of having many ways to "see" an attacker, no matter where they are in your environment. It increases your chances of catching threats early and reducing potential damage, even when prevention fails.
**Detection-in-depth provides comprehensive detection and monitoring by placing monitoring, alerting, and logging mechanisms at every level:**
- At the **perimeter** (firewall logs, intrusion detection systems),
- Within the **network** (traffic analysis, segmentation alerts),
- On **critical systems** (endpoint protection, change detection),
- And around **user activity** (access logs, behavioral monitoring).
### Cyber Risk
**Cyber risk** is the **possibility** that a business's information systems will be **compromised** by **unauthorized access, use, or destruction**. The frequently used **risk equation** below not only accounts for **threats** but also considers **vulnerability** (how exposed the IACS is) and **consequence** (the maximum potential damage).
#### **Risk = Threat x Vulnerability x Consequence**
### Risk Tolerance
**Risk tolerance** refers to the **level of risk an organization is willing to accept** to pursue its security objectives. It reflects the amount of uncertainty or potential loss that management is comfortable with. It **considers the likelihood of risk and its possible impact**.
A good risk assessment process will identify the types of controls that need to be implemented to minimize risk.
### Risk Response Strategies
![[Pasted image 20260427130308.png]]
If a cyber threat is revealed through a risk assessment or other means, management can respond with different strategies depending on the potential likelihood and impact.
### Risk response strategies
- Avoid - Eliminate the risk by redesigning or changing ineffective controls, plans, or processes.
- Transfer - Action is taken to decrease risk severity by either implementing controls or sharing risk between different parties.
- Reduce - Reduce means lowering the likelihood or impact of a risk—not eliminating it.
- Accept - Accepting the risk means keeping the risk and developing contingency plans to cover the consequences if an event occurs.
# 2. Awareness
According to ISA/IEC 62443, **cybersecurity should receive the same emphasis as safety and operational integrity** because the consequences can be just as severe. In the complex world of [[IACS]], cybersecurity isn't just about firewalls and passwords. It's also about people.
The standard recognizes that the human element is both a vulnerability and a defense. It calls on organizations to train all personnel—not just IT staff—on their roles in securing the [[IACS]] environment. Whether it's understanding phishing risks, proper password hygiene, or incident reporting procedures, **awareness creates the first line of defense**.
![[Pasted image 20260427133109.png]]
### Effective Awareness Training 
1. Audience - targeted training for your audience. Programs should be role-based.  
2. Customization - Tailor the awareness activities, so they relate to your context and applicable policies. 
3. Reinforcement - one - off sessions aren't enough. The standard promotes continuous learning and regular updates. 
### Examples of IACS-specific awareness activities
- Red team/blue team training using a realistic simulation of the organization's IACS environment .
- Demonstration of Industroyer malware on protection relay at electricity grid operator, causing malfunction of critical grid functionality.
- E-learning for all OT and IT staff with a questionnaire at the end. 
- Board Member session that uncover high-impact IACS cybersecurity risks and how they affect the business
# 3. ISA/IEC 62443 Series
## Structure of ISA/IEC 62443
The **ISA/IEC 62443 series** is a **comprehensive set of standards, technical reports (TR),** and related information **designed to** **secure Industrial Automation and Control Systems (IACS)**.
The official designation for the standards is either “IEC 62443” or “ANSI/ISA-62443”, depending on which edition is purchased. For convenience, we recommend the less formal designation **“ISA/IEC 62443”** to highlight that **both editions are identical in content**. Also, note that for the ISA editions, the “ANSI/” prefix applies only to standards and not technical reports.
The chart below outlines the goals of the ISA99 Standards Committee.  Not all of these standards, technical reports, and technical specifications are published.
The standard series includes **six groups,** each **targeting different aspects and stakeholders** within the industrial environment.![[Pasted image 20260427134913.png]]
### ISA/IEC 62443  |  Standards and Technical Reports
I**SA/IEC 62443** includes **standards** and **technical reports.** It includes over 400 normative requirements and 150 requirement enhancements.
**Standards** are **prescriptive** and use **shall or must** statements.  They are prescriptive, meaning they **provide requirements, directions, or recommendations about what should be done.**
**Technical reports (TRs)** are **informative publications** that **provide detailed data, process methodology, or other information on a particular technical subject.** They look like standards, but they are **descriptive**.  They do not use any shall or must statements.
### ISA/IEC 62443 Groups
**The 62433 standards and technical reports** are arranged in **six groups**, corresponding to the **primary focus** and intended **audience**. You should be able to identify these groups and their primary focus. [[ISA/IEC 62443 Groups]]
### IACS Cybersecurity Roles 
In the world of industrial automation, cybersecurity isn't just a technical necessity - it's a collaborative mission. The ISA/IEC 62443 standard provides the roadmap, but it's the people across roles who bring it to life.
Roles that are identified in the ISA/IEC 62443 Series:
- **Asset Owner** is accountable and responsible for the IACS. the Asset Owner is also the operator of the IACS and the Equipment Under Control.
- **Maintenance Service Provider** provides support activities for an  Automation Solution.
- **Integration Service Provider** provides integration activities for an Automation Solution including design, installation, configuration, testing, commissioning, and handover.
- **Product Supplier** manufactures and supports a hardware and/or software product. Products may include Control Systems, Embedded Devices, Host Devices, Network Devices, and/or Software Applications. 
It is important to understand that a role is not necessarily an organization. An organization can have multiple roles, and the responsibilities for a particular role can be split among multiple organizations.
### Mapping roles to standard parts
This diagram maps each role in the IACS security environment to the specific ISA/IEC 62443 standard parts they are most likely to use. As you can see, there is overlap where Parts 1-1, 2-3, and 3-3 are used by The Profiles parts of the standard provide ready-to-use implementation guides which could apply to any role.  The Evaluation parts cover conformity assessment which would be used by evaluators.
![[Pasted image 20260427140334.png]]
# 4. ISA/IEC 62443 Models And Security Levels
## ISA/IEC 62443 Models
ISA/IEC 62443 relies on various **model types** to help **standardize communication**. A **reference** model describes a **generic view** of an **integrated** manufacturing or production **system**. The **asset model**, reference architecture model, and **zone** model, provide the details needed to address security issues.
### Model Types
- [[Reference Model]] - Provides the overall conceptual basis for the more detailed models to follow.
- [[Asset Model]] - Defines the relationship between assets within IACS.
- [[Reference Architecture]] - Describes the asset configuration and can be unique to each enterprise or its subsets.
- [[Zone Model]] - Groups reference architecture elements according to defined characteristics. 
This diagram illustrates the interconnection of models within the security program. Models don't work in isolation. They support and interact with the policies, procedures and guidelines, and are then applied to the assets, contributing to a cohesive security strategy. This framework guides the development and implementation of security measures across the system.
![[Pasted image 20260427142645.png]]
### Policies, procedures and Guidelines
Understanding the purpose of **_policies, procedures, and guidelines_** is crucial in cybersecurity and risk management. These elements form the foundation of a **strong security framework** by ensuring that everyone knows what to do, how to do it, and why it's important.
They **reduce risks** by ensuring everyone follows **proven security practices**.
They support **compliance** with **laws and regulations.**
They help build a **unified, proactive security culture**.
![[Pasted image 20260427145046.png]]
### Policy 
Establishes the overarching direction.
- Defines mandatory rules for protecting sensitive and critical system resources.
- Serves as the organization's standard against which security audits measure compliance.
### Procedure 
Defines how to carry out the direction.
- Defines in detail the sequence of steps necessary to implement a certain security measure. 
- Policies reference procedures and mandate their use.
### Guideline
Provides flexible but recommended best practices.
- Describes a way to do something that is desirable but not mandatory.
- Cannot be audited for compliance, as they are advisory and not enforceable. 
## Security Levels 
**Security levels 0 to 4** refer to a tiered classification of **system or network security requirements**. These levels are cumulative, meaning each level builds upon the protections of the previous one. **Each level requires greater security measures** and assumes more capable adversaries. Choosing the right level depends on the **risk assessment, asset value, and threat landscape**.
![[Pasted image 20260427155612.png]]
# Security Levels
## SL 0 - No Specific Requirements 
Key Point: No security at all.
- Systems at this level do not resist intentional security threats.
- May have safety mechanism, but no cybersecurity protections.
- Suitable for non-critical systems with isolated operations.
## SL 1 - Protection Against Casual or Accidental Violation
Key Point: Basic protection against unintentional or casual threats.
Defends against:
- Unskilled attackers
- Accidental misuse
Focuses on:
- Simple authentication
- Minimal access control
Use case: Small business systems or early - stage ICS deployments
## SL 2 - Protection Against Intentional Violation Using Simple Means
Key Point: Protection from intentional, but unsophisticated threats.
Defends against Hackers with limited resources and Script kiddies.
Includes:
- Role-based access controls
- Basic network segmentation
- Audit capabilities
Use Case: Systems where some cybersecurity awareness is needed, but threats are not highly advanced.
## SL 3 - Protection Against Sophisticated Attackers with Moderate Resources
Key Point: Countermeasures against skilled attackers.
Includes:
- Strong authentication
- Secure communications
- Intrusion detection/prevention
Requires:
- Formal security policies
- Regular security assessments.
Use Case: Critical infrastructure, utilities, or systems subject to advanced persistent threats (APTs)
## SL 4 - Protection Against Sophisticated Attackers with Extended Resources
Key Point: Maximum protection for high - value or national-critical systems.
Defends against State-sponsored actors and Advanced tools and techniques.
Features:
- Hardened systems.
- Continuous monitoring.
- Custom-tailored security architectures.
Use Case: Defense, nuclear plants, or systems requiring resilience against the most advanced threats.
# 5. Introduction To The IACS Cybersecurity Lifecycle
# 6. Security Program (SP) Requirements For Asset Owners
## ISA/IEC 62443 and ISO/IEC 27001
[[ISA-IEC 62443]] and [[ISO-IEC 27001]]/2 are standards that support structured, risk - based cybersecurity governance, but they apply in different environments (IT versus OT).  
ISO-IEC 27001 provides requirements for establishing, implementing, maintaining, and continually improving an Information Security Management System ([[ISMS]]). It includes a list of commonly accepted controls to be used as a reference for establishing security requirements. 
**ISO 27002** provides further detailed guidance for organizations implementing these information security controls. 
ISAGCA's white paper “Applying ISO/IEC 27001/2 and the ISA/IEC 62443 Series for Operational Technology Environments”, which can be downloaded below, provides more details for a deeper dive. 
Organizations seeking end-to-end security across IT and OT often implement both standards, mapping controls between them to avoid duplication and ensure coherence.
![[Pasted image 20260427163608.png]]
## Shift from Cybersecurity Management System (CSMS) to Security Program (SP) Requirements
### Major Shift in ISA/IEC 62443-2-1
A very common engineering approach when faced with a challenging problem is to break the problem into smaller pieces and address each piece in a disciplined manner. This approach, outlined in the previous edition of ISA 62443-2-1,  is sound for addressing cybersecurity risks with [[IACS]]. Many organizations still use this approach.

However, dealing with cybersecurity one system at a time (IT versus OT) has proven to be a common mistake, resulting in unnecessary redundancies and oversights. **Cybersecurity is a much larger challenge that should address all IACS components as well as the policies, procedures, practices, and personnel that surround and utilize those [[IACS]].**

**Significant Changes include:**
- Revised requirement structure into **Security Program ([[SP]]) elements (SPEs)** integrated into a broader Information Security Management System ([[ISMS]])
- Eliminated duplication of ISMS requirements
- Defined a maturity model for evaluating requirements
- Emphasizes securing supply chains and ensuring that external parties adhere to security practices

The updated standard supports the need to address cybersecurity for an IACS in operation by providing **requirements for establishing, implementing, maintaining, and continually improving an IACS Security Program (SP).** When implemented conscientiously, these requirements provide security capabilities that **aim to reduce IACS security risks to a tolerable level**. These requirements are meant to be implemented independently, allowing asset owners to **select approaches most suitable to their needs**. ISA/IEC 62443‑3‑2 1 describes the methodology for addressing cybersecurity risks in an IACS system design, which assists in identifying risks and selecting appropriate security requirements and associated capabilities for an IACS SP.
Being familiar with the key points for both methodologies is important because you may encounter either option at any given organization. 
## Security Program (SP)
###  **Enhanced Alignment & Shared Responsibility**

The updated standard provides **mappings** between:
- **[[SPE - Security Program Elements]]s** (security program elements)
- **[[SR]]s** (system requirements in IEC 62443‑3‑3)
- **[[CR]]s** (component requirements in IEC 62443‑4‑2)
- And even the Security Program requirements for service providers (IEC 62443‑2‑4)

This tight alignment underscores a **shared-responsibility** model across asset owners, integrators, product suppliers, and service providers

###  **Maturity Levels**
The **Maturity Levels ([[ML]]s)** introduced in ISA/IEC 62443-2-1:2024 provide a **benchmarking** **tool** for organizations to assess how well they manage **Security Program Elements** (**SPEs**). The [[ML]]s help guide **incremental improvement** in a structured way, allowing asset owners and auditors to evaluate readiness for implementing security measures.
![[Pasted image 20260427164745.png]]
![[Pasted image 20260427164801.png]]
![[Pasted image 20260427164814.png]]
Each [[SPE - Security Program Elements|Security Program Element]] in the standard is evaluated against these levels. As organizations mature their processes, they aim to move from **ML1** to **ML4** over time. Maturity Levels are not just for compliance—they're a roadmap for building resilient, adaptive cybersecurity programs in industrial environments.
![[Pasted image 20260427164724.png]]
## Conformance and Assessments
The updated 2024 version of the standard replaces inflexible technical mandates with **a maturity approach**. To achieve conformance, asset owners must define Security Program Elements (SPEs), then demonstrate implementation, monitoring, and continuous improvement, proving they meet performance objectives without dictating exact controls.
The standard recognizes that many IACS systems are 20+ years old. If **legacy components** lack update/patch support, owners **must** **document compensatory policies and procedures to mitigate risk**.
While asset owners hold ultimate responsibility, they must **enforce security clauses** in contracts with integrators and product suppliers, aligning those parties with **SPE requirements**.
- Conformance - Evaluates, applies, and documents methods in each requirement of the applicable IEC 62443 series part, mitigating security risks and providing supporting evidence for all identified processes.
- Assessment - Measures conformity with requirements through verification or validation processes, either internally or via a third-party process compliant with [[ISA-IEC 62443]], verified by providing supporting evidence.
- Conformity Assessments - Can be self-assessments by assets owners, service providers, or product suppliers using internal processes, or independent third-party assessments.
###  **Conformity Evidence**
Proof of conformity and conformance methods can be provided in many forms. Most requirements identify supporting evidence by outlining the specific methods that include, but are not limited to:
- Verifying the use
- Capability and configuration of technology
- Supporting processes
- Validation through testing of capabilities
Evidence types that can be used to prove conformity are identified in the table below.
![[Pasted image 20260427165339.png]]
![[Pasted image 20260427165355.png]]
### [[SPE - Security Program Elements]]
# 7. Evolving Security Standards And Practices
## Regulations
### Industry Regulations
**Regulations** are **legally enforceable rules** created by government bodies or authorized organizations that dictate specific requirements and behaviors. Non-compliance results in penalties, fines, or legal actions.
### Mandatory Compliance
**Mandatory compliance** refers to the legal obligation for an organization or individual to follow specific laws, regulations, or binding requirements. Failure to meet these obligations can lead to penalties, such as fines, legal action, or even loss of operational licenses.
### Enforced by Law
Failure to comply can result in civil or criminal penalties, and courts may determine liability or negligence without relevant regulations.
Holds organizations accountable for failing to meet basic safety or security standards based on what a reasonable person or organization would do in a similar situation.
### Enforcement and Oversight
**Regulatory bodies monitor compliance** and can conduct inspections, audits or investigations to ensure adherence.
### Additional Aspects of regulations 
![[Pasted image 20260428102515.png]]
### Summary 
Securing Industrial Automation and Control Systems (IACS) involves complying with various regulations, standards, and guidelines, many of which are region-specific or industry-specific.
1.  **ISA/IEC 62443** is the cornerstone standard for IACS security.
2.  **NIST SP 800-82 and NERC CIP** provide U.S.-specific guidance, especially for critical infrastructure.
3. **EU NIS2 Directive** drives regulation across Europe, emphasizing incident reporting and risk controls.
4. **Compliance varies by sector and geography, but the core goals remain the same: reduce risk, enhance resilience, and protect operational technology (OT).**
## Global frameworks
**A** **framework** **is a structured approach that helps organizations manage and improve their cybersecurity practices while offering clear guidelines, best practices, controls, and processes.**
It describes “what” an organization will do to manage security risks (i.e., blueprint/roadmap)
A framework provides a common taxonomy and mechanism to:
1. Assess current cybersecurity posture
2. Define a target state for security  with desired outcomes
3. Identify and prioritize risks and opportunities for improvement within the context of a continuous and repeatable process
4. Measure progress toward the target state
5. Communicate among internal and external stakeholders about cybersecurity risk and strategies
## NIST Cyber Security Framework (CSF)
The [[NIST Cyber Security Framework (CSF)]] uses informative references like ISA/IEC 62443 to **help organizations protect critical assets and data from cyber threats**.
The NIST CSF:
- **Offers flexible guidelines** that can be tailored to any organization, regardless of size or industry.
- **Promotes continuous improvement and resilience** **in cybersecurity practices.**
## Summary 
### Continuously Monitor and Evaluate Applicable Legislation
1. Organizations should routinely review, improve, and maintain their [[CSMS]] to ensure its effectiveness against evolving risks. They **should** monitor and evaluate industry CSMS strategies to stay updated on best practices, emerging threats, and improvements. Organizations **shall** monitor and evaluate applicable legislation relevant to cybersecurity to ensure compliance with legal requirements as new laws are introduced or existing ones evolve.
2. The NIST CSF Framework includes informative references, which are **globally** recognized standards such as ISA/IEC 62443 and ISO 27001.
3. By aligning ISA/IEC 62443 and NIST CSF, countries and industries can work together to secure critical systems and improve global cybersecurity resilience.
![[Pasted image 20260428120716.png]]
# 8. Network Security Basics
## Why We Address Security in IACS
**TCP/IP was built for functionality, not security.**
It was developed to ensure reliable communication across networks.
Protocol developers assumed communications would occur in a trusted environment, but the design actually leaves it vulnerable to attacks that could disrupt services, compromise data, and lead to unauthorized access

**PLCs were built for control and operational efficiency, not defense.**
PLCs were introduced to replace relays and manage I/O operations (control physical processes by servicing inputs and outputs).
Ethernet connectivity was added later as an afterthought.
PLCs were not designed to defend against cyber threats. Many lack authentication mechanisms and are vulnerable to firmware exploitation.

## Open Systems Interconnection - [[OSI Model]]
## MITRE ATT&CK Framework For ICS
ATT&CK, Adversarial Tactics, Techniques, and Common Knowledge, is MITRE's knowledge base for modeling cybersecurity threats based on real-world incidents. It is specifically designed for threats against industrial control environments rather than IT and explains how attackers infiltrate, operate within, and affect industrial systems.
Organizations can use the framework to map their defenses against known tactics and techniques to understand, detect, and mitigate threats across IT and OT environments. It standardizes threat intelligence, supports realistic attack modeling, and prioritizes defenses that protect critical industrial processes and safety functions. It also integrates with other security frameworks such as ISA/IEC 62443, NIST CSF, CIP, and more.
The ATT&CK matrix is a visual table that organizes tactics and techniques.
Tactics (columns) — the adversarial goals or "the why"
Techniques (rows) — methods used or "the how"
## [[Network Security Technologies in IACS]]
## Intrusion Detection Systems - [[IDS]]
## Intrusion Prevention Systems - [[IPS]]
![[Pasted image 20260428124435.png]]
## More Network Security Tools
### Unified Threat Management - [[UTM]]
### Virtual Private Network - [[VPN]]
## Network segmentation
### Business/Process Firewall Architecture
**Network segmentation** is the practice of dividing a computer network into **smaller, separate sections**, each with its **own rules and controls** to improve security and performance.
A **strong firewall is essential for creating a secure boundary** between the industrial/OT network and the broader IT network (between the plant floor and the rest of the company network). This **ensures** **plant operations remain isolated and protected from external vulnerabilities.**
**Routers are not designed to provide robust security** as they lack the capability to detect threats, control access, and inspect firewall traffic.
### [[DMZ]]
### One firewall, or two?
![[Pasted image 20260428125357.png]]

# 9. Industrial Protocols
# 10. Introduction To Patch Management
# 11. Introduction To Security Risk Assessment For System Design
# 12. Security Program Requirements For IACS Service Providers
 **This part of the ISA‑ 62443 series defines requirements for security capabilities to be supported by security programs of integration and maintenance.**
Support for these capabilities means the **service provider can provide them to the asset owner** upon request.
In addition, **ISA‑ 62443-2-4 can be used by these service providers** to structure and improve their security programs.
## What is a service provider?
A service provider is an individual or organization that **provides a specific support service and associated supplies,** generally as an agreement with the asset owner. A service provider does not need to be a separate individual or organization (a separate legal entity). Many larger Asset Owners have internal departments that fulfill the service provider role.
There are **integration and maintenance service providers.** The concept also includes **product suppliers.** In the 62443 standards, provider and supplier terms are used in place of the generic word vendor to provide differentiation.
## Types of IACS Service Providers
### Integration Service Provider
An IACS Integration Service Provider provides the capabilities to implement/deploy automation solutions according to asset owner requirements. 
Integration service provider activities generally occur starting with the design phase and ending with the handover of the automation solution to the asset owner.
Typical Integration Service Provider Activities include:
- Defining the technical specifications that guide the integration
- Assessing system requirements and designing tailored solutions
- Installation, configuration, patching, backup, and testing of systems
- Gaining approval of the asset owner during the execution of activities
### Maintenance Service Provider
**An IACS Maintenance Service Provider performs activities that maintain and service Automation Solutions according to asset owner requirements.**
Maintenance activities are separate from operational activities.
Maintenance activities generally start after the handover of the Solution.
They may continue until the asset owner no longer requires them.
**Typical Maintenance Service Provider Activities include:**
- Patching and anti-virus updates
- Equipment upgrades and maintenance
- Component and system migration
- Change management
- Contingency plan management
### Product Supplier
A product supplier manufactures a hardware and/or software product.
The product supplier develops control system products as a combination of:
- Supporting applications
- Embedded devices
- Network components
- Host devices
The products are independent of an IACS environment.
Maintenance activities may be shared by:
- Asset Owner
- Integrator
- Maintainer
- Product Supplier
## ISA/IEC 62443-2-4 Security Program Functional Areas
In order to claim conformance, Service Providers must adhere to the many requirements in ISA/IEC 62443 Part 2-4.
Conforming to these requirements can give service providers a competitive advantage in the markets in which they operate. As more asset owners ask for ISA/IEC 62443 conformance while contracting service providers, this shows that they integrate cybersecurity into their day-to-day work for the asset owner.
This table shows the twelve categories or functional areas that have been defined to group these requirements. It provides a high-level summary of the areas in which Service Providers can claim conformance.
![[Pasted image 20260428132236.png]]
## **Evaluating Security Program Requirements for IACS Service Providers**
**ISA/IEC TR/TS 62443-6-1** was published in 2024. **The technical report (TR) contains objective evaluation criteria**. It **supports** service providers and evaluators who conduct **conformity assessments by evaluating the security program against the requirements of ISA/IEC 62443-2-4.**
Per the requirement of ISA/IEC 62443-2-4, the evaluation criteria and what evidence needs to be provided per maturity level (ML 1 to ML 4) are established.
**The goal is to achieve repeatable and reproducible evaluation results**.
# 13. Developing Secure Products And Systems
# 14. Security Profiles For ISA 62443
## **IEC Technical Specification 62443-1-5**
This technical specification **outlines a scheme or framework for developing cybersecurity profiles within the ISA/IEC 62443 series.**
**The scheme contains the steps to produce a profile and its required contents**. It assures that cybersecurity profiles are created with the necessary degree of **uniformity.**
Cybersecurity profiles created using this scheme will be published as subparts of the ISA/IEC 62443-5 series.
These **profiles serve as a guide for stakeholders to adopt a specific set of requirements** defined in the ISA/IEC 62443 series.
 It facilitates the application of **standardized ISA/IEC 62443 terminology**, such as roles, and **allows for the tailored interpretation of requirements specific to various industry sectors or application areas.**
This capability significantly enhances the effectiveness of implementing ISA/IEC 62443 standards across distinct verticals.
## Security Profiles
A **security profile** is a structured way to tailor the standard's general cybersecurity requirements to a specific industry, application, or environment.
### **Sector-specific**
A security profile **selects, modifies, or prioritizes the standard’s foundational requirements (FRs) and system requirements (SRs) based on the needs of a particular sector**, like electric utilities, oil and gas, or water treatment.
The profiles help organizations **apply the horizontal (broadly applicable) 62443 standards in a vertical-specific context** (e.g., electric energy OT systems).
Each security profile **defines which controls are mandatory, optional, or not applicable**, making implementation more relevant, efficient, and aligned with actual risk.
## **Scheme/Framework for Cybersecurity Profiles**
**Security profiles must adhere to established guidelines** to prevent unnecessary variations in new or modified requirements. Scheme requirements include the following:
- Security profile shall **refer to single or multiple ISA/IEC 62443 documents**
- Documents that can be referred to are **ISA/IEC 62443-2-1, 2-4, 3-3, 4-1, and 4-2**
- Included **requirements will be identified, and require justification for those excluded**
![[Pasted image 20260428133605.png]]
## **Profile Example: A work in progress**
Within the **US Department of Energy**, the Secretary of Energy established a working group composed of senior government, industry, and nonprofit representatives as mandated by Sec. 5726 of the 2020 NDAA.  With a **defense-in-depth mindset**, they started developing the following **reference architecture (RA)**. ISA contributed to the effort, and **ISA99 Working Group 14 continues the effort today**.
**The design is:** 
- **Specifically for the electrical sector**
- **Not limited** to localized industrial processes
- **Focused** on properties of information passing between devices
- **Flexible** enough to reflect advances in technology and design practices.
As a result, the **Reference Architecture(RA) for Electric Energy OT** was created, **from which other domain-specific profiles could be derived**: specific profiles for substation (seen below), generation, distributed energy resources, and operation/network control center. It can serve as a template or starting point.
It helps **individual grid operators use a common profile** and enables a **common protection level** across the sector. **Product suppliers** also know what requirements will be asked for in that sector. It brings the entire sector closer together regarding the use of the ISA/IEC 62443 standards.
# 15. IACS Security Protection Scheme

# Keywords
- Asset
- Threat
- Vulnerability
- Risk
- Countermeasure
- Zone
- Conduit
- Security Level (SL)
	- SL-T (Target)
	- SL-A (Achieved)
	- SL-C (Capability)
- Defense in Depth
	- Policies
	- Users
	- Applications
	- Systems
	- Networks
	- Physical Security
- Least Privilege
- Attack Surface
- Fundamental Requirements
	- FR1 - Identification and Authentication Control
	- FR2 - Use Control
	- FR3 - System Integrity
	- FR4 - Data Confidentiality
	- FR5 - Restricted Data Flow
	- FR6 - Timely Response to Events
	- FR7 - Resource Availability

#szkolenie1B 