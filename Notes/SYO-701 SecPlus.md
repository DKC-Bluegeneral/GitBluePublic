# __CompTIA SYO-701 Security + Study Notes__




<p align="center">
  <img src="https://github.com/DKC-Bluegeneral/Notes/blob/main/Images/CompTIASecPlus.jpeg" alt="DKC-Bluegeneral">
</p>





# Disclaimer:  These are not comprehensive notes. These are a rough draft of class notes, and study notes, I will remove this when they are complete.










# Domain 1:Threats, Attacks, and Vulnerabilities
# Domain 2: Technologies and Tools
# Domain 3: Architecture and Design
# Domain 4: Identity and Access Management
# Domain 5: Risk Management
# Domain 6: Cryptography and PKI (Public Key Infrastructure)


`Don't forget to sort by domain later`
















# Gap Analysis


- Know where you are, and where you need to go.


## Common gaps:


- Weak credentials or shared credentials
- Lack of tested patch management
- Violation of least privilege principle
- Having no/unenforced acceptable use policies
- Poor physical security
- Configuration and deployment errors due to lack of change and configuration management
- Poor visibility and lack of proper auditing





# Zero trust control plane





## Zero Trust (ZT):


- ZT assumes there is no implicit trust granted to assets to user accounts based solely on their physical or network location based on asset ownership. 

- Segregation of duties and high visibility are also emphasized 

- Adaptive identity is another key ZT component. It’s also called adaptive authentication, or risk based authentication. It is  a method of access to data that matches user credentials with the risk of the requested authorization. 

- Zero Trust Control Plane is separate from the data plane, and contains the policy decision point (PDP), which includes:
The Policy engine (PE), which uses the enterprise policy-driven access control panel (as well as input from external sources) to grant, deny, or revoke access to resources. 
The policy administrator (PA) which enables or shuts down the communication path between subject and a resource  via commands to associated policy enforcement points (PEPs)

- The PA communicates with the PEP when creating the communication path via the control plane. 





# CIA Triad





## Confidentiality


- Confidentiality ensures that information is accessible only to those who are authorized to view or use it. It involves protecting sensitive data from unauthorized access, disclosure, or interception. Measures such as encryption, access controls, and data classification help maintain confidentiality.


## Integrity


- Integrity ensures that information remains accurate, complete, and trustworthy throughout its life-cycle. It involves protecting data from unauthorized modification, deletion, or corruption. Techniques such as checksum, digital signatures, and access controls help verify data integrity and prevent unauthorized changes.


## Availability


- Availability ensures that information and resources are accessible and usable when needed by authorized users. It involves maintaining continuous and reliable access to systems, networks, and data, even in the face of disruptions or attacks. Redundancy, backups, disaster recovery plans, and fault-tolerant systems are used to maximize availability and minimize downtime.


### Non-Repudiation


- Enforcing the inability of a subject to deny that they participated in a digital transaction, agreement, contract, or communication such as an email.

- Non-repudiation is the property of agreeing to adhere to an obligation

- More specifically, it is the inability to refute responsibility.





# Authentication, Authorization, and Accounting





## Authentication


- The process of validating that an entity (user, application, or system) is who or what they claim to be

## Authorization


- The process of granting an authenticated entity permission to access a resource or perform a specific function

## Accounting


- Basically, when did the entity begin, when did it end, and how long did they do it?





# Character vs Packet Mode





## Character Mode


- In networking, character mode refers to a method of data transmission where individual characters or bytes are sent and received sequentially. Each character is transmitted independently, and there is no inherent structure or formatting imposed on the data stream.


## Packet Mode


- Packet mode, also known as packet-switched mode, is a method of data transmission where data is organized into packets before being transmitted over a network. Each packet contains both data and control information, including source and destination addresses, error checking codes, and sequencing information.





# Authorization Models





## DAC (Discretionary Access Control):


- Discretionary Access Control grants access controls decisions to the resource owners and custodians.

- Each resource typically has an owner who determines the access permissions and shares.

- The owner can grand or revoke access rights for other users or groups.

- DAC is flexible and allows owners to have fine grained control over access, but it can also result in inconsistant access control desisions.

- **MOST PRONE TO PRIVELEGE CREEP**


## RBAC (Role-based Access Control):


- Grants access based on predefined job role or title.

- Users are assigned roles, and access rights and are associated with these roles.

- Instead of directly assigning permissions to individual users, permissions are assigned to roles, and users inherit the access rights associated with their assigned roles, for example:

	- Various Roles in a hospital or medical center

	- Built-in roles in a database management system

	- RBAC streamlines access control administration by grouping users with similar job functions and offering scalable approach to access management.

	- Can be mixed with other models for ease of use


## MAC (Mandatory Access Control):


- A Strict mathematical model where access to resources is determined by the system based on predefined security labels and rules.


- Principals are assigned security clearances or classification levels (Top Secret, Secret, Confidential, Etc.)


- Resource objects are labeled with sensitivity levels

- Access is granted or denied by comparing these labels and rules, ensuring strict control and preventing unauthorized access.

- This is a "Non -Discretionary" model:

	- A non-discretionary model refers to a security policy where access control decisions are determined by system administrators or security administrators rather than by individual users.

	- In non-discretionary models, users do not have the discretion to modify or override access control settings for resources.

	- Access decisions are typically based on predefined rules, such as security labels or classifications assigned to users and resources, rather than on user-defined permissions.

	- This approach helps enforce strict access controls and reduces the risk of unauthorized access or data breaches.


## ABAC (Attribute-based Access Control):


- Grants access based on a combination of characteristics associated with users, resources, and environmental conditions. 

- Attributes could include:

	- User Attributes (Job Title, Department, Etc)

	- Resource Attributes (Sensitivity level, classification, etc.)

	- Environmental attributes (time of access, location, etc.).

- Authorization policies are defined using these combinations, and decisions are made based on evaluating the attributes against the defined policies.


## ABDAC (Attribute-based dynamic access control):


- Combines principals of ABDAC and DAC.

- Considers dynamic factors such as risk assessment, user attributes, resource attributes, and contextual information to make access control decisions in real time.

- ABDAC provides more fine-grained and context-aware access control needed in "zero-trust" environments when compared to other more static access control models.

- May include dynamic machine learning techniques such as user behavioral analytics (UBA) in next generation environments. 


## RBAC (Rule-based Access Control):


- Access control rules define conditions or criteria that must be met for access to be granted.

- Rules can be based on several factors, such as user attributes, resource attributes, time of access, and more.





# Control Categories





## Technical Controls:


- These controls involve the use of technology to protect information systems, networks, and data. Examples include:

	- Firewalls, encryption, access controls, antivirus software, IDS, SIEM, and SOAR.


## Managerial Controls:


- These controls focus on policies, procedures, and administrative measures to manage and oversee security within an organization. Examples include:

	- Security policies, risk management processes, security training and awareness programs, and incident response plans.


## Operational Controls:


- These controls deal with the day-to-day operational aspects of security, including the implementation and enforcement of security policies and procedures. Examples include:

	- Access control procedures, backup and recovery processes, change management procedures, and system monitoring.


## Physical Controls:


- These controls involve measures to protect physical assets, facilities, and resources from unauthorized access, damage, or theft. Examples include:

	- Locks and keys, access control systems, surveillance cameras, perimeter fencing, and environmental controls such as fire suppression systems.





# Control Types





## Preventive Controls:


- These controls aim to prevent security incidents from occurring by implementing measures that stop or minimize the likelihood of threats and vulnerabilities being exploited. Examples include:

	- Firewalls, access control lists, encryption, and security awareness training.


## Deterrent Controls:


- Deterrent controls are intended to discourage potential attackers from attempting to exploit vulnerabilities by increasing the perceived risk or effort required. Examples include:

	- Security signage, visible security cameras, and security patrols.


## Detective Controls:


- Detective controls are used to identify and detect security incidents or breaches after they have occurred. These controls help in monitoring and alerting security teams to abnormal or suspicious activities. Examples include:

	- Intrusion detection systems, security logs and auditing, and security incident response teams.


## Corrective Controls:


- Corrective controls are implemented to mitigate the impact of security incidents and restore systems to their normal functioning state. These controls aim to address the root cause of the issue and prevent similar incidents from occurring in the future. Examples include:

	- System backups, patch management, and incident response procedures.


## Compensating Controls:


- Compensating controls are alternative measures implemented to provide an equivalent level of security when primary controls cannot be implemented or are ineffective. These controls help in mitigating risks and maintaining security posture. Examples include:

	- Multi-factor authentication, compensating controls for legacy systems, and security monitoring tools.


## Directive Controls:


- Directive controls establish policies, guidelines, and procedures to direct behavior and actions within an organization to ensure compliance with security objectives. These controls provide guidance on security requirements and expectations for employees and stakeholders. Examples include:

	- Security policies, standards, and procedures, security training programs, and access control policies.





# Privilege Escalation





- This is more of a phase for a multi-stage attack, not just an attack it's self. 

- Privilege escalation can occur during the attack, part of the kill chain, or during pen-testing

- Can be vertical or horizontal.

- APT (Advanced Persistent Threats) often attempt an escalation of access privileges soon after the initial compromise phase. 

- The goal is to become the root/admin user on the device

- Least privilege is key

- Having current versions of all software (OS, applications, etc) can help mitigate this.

- SUID (Set User ID `SUDO`) It is a special permission in Unix-like operating systems that allows users to execute a file with the permissions of the file's owner or group, rather than with the permissions of the user who is executing it.





# Cross Site Scripting (XSS)




- **XSS**

	- Flaws in pages rendered by web servers and not the web server code itself (i.e. Apache, IIS) where malicious scripts or code are injected into trusted or innocent web site pages.

	- Malicious scripts can steal cookies, session tokens, or other sensitive data stored by the browser and used with the site.

	- Attacker typically sends browser-side scripts to end user.

	- Can occur anytime a web program uses user input within the output it generates without validating or encoding.


## XSS Types:


- **DOM (Document Object Model) Based XSS (Local or Type 0):**

	- In this type of XSS attack, the malicious script is injected and executed client-side by modifying the DOM  directly.

		- Example: An attacker modifies the URL parameter `?name=<script>alert('XSS')</script>` on a vulnerable webpage. The script modifies the DOM to display an alert when the page loads, executing the attack on the user's browser.

- **Reflected XSS (Non-persistent or Type 1):**

	- In a reflected XSS attack, the malicious script is embedded in a URL or input field, and the server reflects the injected script back to the user's browser without proper validation or encoding.

		- Example: An attacker crafts a phishing email containing a link to a vulnerable website with the payload `http://vulnerable-site.com/?search=<script>alert('XSS')</script>`. When the victim clicks the link and the search parameter is reflected on the page without sanitation, the script is executed in the victim's browser.

- **Stored XSS (Persistent or Type 2):**

	- Stored XSS occurs when the malicious script is permanently stored on the target server, typically in a database or user-generated content, and is then served to other users who access the affected page.

		- Example: An attacker posts a malicious script as a comment on a blog or forum, such as `<script>alert('XSS')</script>`. When other users visit the page containing the comment, the script executes in their browsers, potentially compromising their accounts or stealing sensitive information.


## Request Forgery (CSRF/XSRF)


- Attack forces an end user to perform undesirable actions in a web application in which they are authenticated

	- An effective CSRF/XSRF attack can force users to perform state-changing requests such as:

		- Transferring Funds

		- Changing their E-Mail address

		- Changing their password

- If a victim is an admin account, the CSRF attack can compromise the entire web application. 


# Injection Attacks


- Often a result of MITM (Man in the middle) or RAT (Remote Access Tool).

- Malware can inject false MAC or IP addresses.

- DLL injection is where malicious code forces its-self to run in place of other benign code.

- This "Injected" code is usually code written by a third party developer, designed to perform some malicious function


## SQL Injection


- Involves inserting a SQL query through input data from client to server application and can allow for several exploits. 

	- Read from sensitive data

		`SELECT FROM`

	- Change database data

		`INSERT, UPDATE, DELETE`

	- Execute administrative functions 

		`shutdown DBMS`

	- Run commands on an operating system


## LDAP Injection (Lightweight Directory Access Protocol)


- Often used in web applications over the internet or a corporate intranet

- The web applications take the input from the client in order to process it further, so the attacker exploits the data not being properly sanitized or going directly to a back-end database. 

- The attacks can render sensitive user information or change information in the LDAP directory. 


## XML Injection


- Also known as "SOAP Injection"

- User input is inserted unsafely

- XML meta-characters can be used to modify

- Can interfere with application logic

- Performs unauthorized tasks or accessible data. 





# Targeted Coding Attacks





## Pointer/object de-reference

- An attacker can supply a pointer for memory locations that the program is not expecting

- A Null-pointer de-reference occurs when a pointer with a value of NULL is used as if it actually points to a valid memory area

- A program can possibly de-reference a null pointer, and in doing so, raise a NullPointerException

- Null pointer errors are frequently the result of one or more programmer assumptions being violated. 

## Directory Traversal

- Also known as a path transversal attack or a "Dot Slash" and is most often launched through a web browser and other clients.

- This HTTP exploit allows and attacker to access restricted files, directories, and commands located outside of the root directory

- Attackers can modify a URI or URL to force the web server into exposing the restricted files.

	- Examples Include:

		![Example 1](https://raw.githubusercontent.com/DKC-Bluegeneral/Notes/main/Images/Dir-Transversal-Example-1.png)


## Buffer and Integer overflows


- **Buffer Overflows**

	- Attacker Sends larger than expected input, for example when a server accepts it and writes to memory areas.

	- Associated buffers are filled and adjacent memory is overwritten as a result.

	- This overwrite may contain instructions or code that crashes the server resulting in a DoS.

- **Integer Overflows**

	- A Type of an arithmetic overflow error when the result of an integer operation does not fit  within the allocated memory space.

	- Instead of an error in the program, it usually causes the result to be unexpected.

	- These are in the top 10 of the most dangerous software errors, mostly because they often lead to buffer overflows.

## Race Conditions - time of check/time of use

- **Race Condition**

	- A race condition is when a system or software tries to do two or more things simultaneously, but due to the type of system, the operations must be done in the correct sequence in order or function properly.

	- Race conditions are classically related to synchronization errors in software code.

	- Crackers can leverage a known race condition vulnerability to get unauthorized access to a system or network.

- **Time-Of-Check vs. Time-Of-Use (TOC/TOU)**

	- A time-of-check vs time-of-use attack is a race condition and occurs when an attacker tries to gain privilege to a system by "racing" it to a resource it is attempting to access.

	- The types of programming flaws that allow for race conditions occur when the system (or application) splits up the operations of verifying credentials and providing access to a resource.

	- It can do things such as replacing a config.sys file with a different file that compromises the system before the system even loads it's operating system.

- **Improper error handling**

	- Poorly defined validation rules used in verifying the correctness, completeness, and acceptability of input data.

	- Software applications and web servers are notorious

	- Must establish data input, data flow, and data output requirements with a designed security features in mind.

	- Collisions are in this category when the chance that two unique inputs will produce the same output (MD5 and SHA-1 are vulnerable)

- **Session replay attacks**

	- Often part of MITM attacks.

		- Examples include:

			- An attacker steals an ID of a user and reuses it to impersonate an authorized user.

			- Web applications that allow reusing old session ID's or session credentials for authorization are also vulnerable to these attacks.

	- IPsec (Internet Protocol Security) and TLS (Transport Layer Security) have anti-replay mechanisms to protect secure session.





# API Attacks




- Application Programming Interface Attacks:

	- An API DDoS attack often involves sending traffic from many clients to overwhelm the API service

	- Even if rate limiting controls are in place to prevent servers from crashing, they cannon always prevent service disruption and severe degradation of the API's user expierence.

	- If API calls are not digitally signed or if they have embedded credentials, they can be compromised.


## API Attack Vectors

- Login Attacks

	- Login attacks involve attempting to gain unauthorized access to an application or system by exploiting weaknesses in the authentication mechanism. This may include brute-force attacks, credential stuffing, or phishing attacks targeting user credentials.

- DDoS Attacks

	- DDoS (Distributed Denial of Service) attacks aim to disrupt the normal operation of an application or service by overwhelming it with a large volume of traffic from multiple sources. This flood of traffic consumes the target's resources, making it inaccessible to legitimate users.

- Leverage Credentials

	- Attackers may leverage stolen or compromised credentials to gain unauthorized access to an application or system. This could involve using leaked credentials obtained from data breaches or phishing attacks to impersonate legitimate users and access sensitive information or perform malicious actions.

- MITM (Man in the Middle)

	- MITM attacks involve intercepting and potentially modifying communication between two parties without their knowledge or consent. In the context of APIs, MITM attacks may target the communication between clients and servers, allowing attackers to eavesdrop on sensitive data or manipulate the transmitted messages.





# SSL Striping and Pass the Hash





## Pass the Hash

- Example:

	- Let's say an attacker gains access to a system and retrieves the hashed password of a privileged user. Instead of cracking the hash to obtain the plaintext password, the attacker can use the hashed password directly to authenticate to other systems where the same password is used. By passing the hashed password, the attacker can potentially gain unauthorized access to additional systems within the network without needing the actual password. This method bypasses traditional authentication mechanisms that rely on verifying plaintext passwords, making it a powerful technique for attackers to escalate their privileges and move laterally within the network.

	- On Windows networks, hackers do not need the plaintext passwords to access certain services.

	- Sometimes the authentication process relies on the passwords cryptographic hash and there are various tools to extract these hashes (Cain) from compromised Windows machines (Lately Windows 10) and use them to access other services.

	- This technique is known as pass the hash and is one of the attacks that windows Virtual Secure Module (VSM) was intended to protect against.

- By definition a Pass the Hash is a vulnerability of Windows Safe Mode.

	- It is an OS diagnostic mode of operation that has been around since windows 95

	- It can be initiated at the boot time and only loads the nominal set of drivers and services that windows needs to run.

	- Most third-party security products do not start up in safe mode so the protection is negated.






# Driver Manipulation





- A Common vector is the hardware drivers that we install in our operating systems

- This is privileged code that is trusted by the OS

- Can be Trojans, RATs, or hacked driver software


## Shimming


- Shimming is the process of stealing information and money from Point-of-Sale (POS) systems, credit card readers, and ATM machines.

- The attack is common at gas stations, convenience stores, and kiosks.

- It can be an overlay attachment or sometimes and entirely replaced device.

	![Example2](https://github.com/DKC-Bluegeneral/Notes/blob/main/Images/ATM-Skimmer-Example-2.png)


## Refactoring

- Involves changing an applications source code without modifying the characteristics.

	- Often used to introduce legacy applications into new computer systems and devices. 

	- Can also re-engineer classic attack code to create variants, hybrid viruses, and worms. 




# Wireless Attacks





## Common Wireless Attacks


- Most malware attacks are multi-phased, stealthy, and polymorphic. Below is a list of some common wireless attacks:


### Evil Twins

- Evil Twin attacks involve setting up a fake wireless access point (AP) with the same SSID (Service Set Identifier) as a legitimate one, tricking users into connecting to it.

	- Examples include:

		- An attacker sets up a rogue AP in a public place, such as a coffee shop, with the same network name (SSID) as the legitimate coffee shop Wi-Fi.

		- Creating a fake Wi-Fi hotspot near an airport with a name similar to the airport's official Wi-Fi network to capture unsuspecting travelers' data.

### Rogue AP

-  Rogue APs are unauthorized access points set up on a network without the network administrator's knowledge or consent, posing a security risk.

	- Examples Include:

		- An employee brings in a personal wireless router and connects it to the company network, providing unauthorized access to outsiders.

		- A hacker installs a rogue AP in a hotel lobby, mimicking the hotel's Wi-Fi network to intercept guests' internet traffic.

### Disassociation

- Disassociation attacks force wireless clients to disconnect from a legitimate AP by sending forged disassociation packets, disrupting their network connectivity.

	- Examples Include:

		- An attacker sends de-authentication packets to users connected to a public Wi-Fi network, causing them to lose connectivity.

		- Disrupting a business's wireless network during a critical meeting by sending disassociation frames to all connected devices.

### Jamming

- Jamming attacks involve flooding the wireless spectrum with noise or interference, disrupting legitimate communication between devices and access points.

	- Examples Include:

		- A malicious actor uses a jamming device to flood the 2.4 GHz frequency band, disrupting Wi-Fi signals in a crowded area.

		- Jamming the frequency used by remote-controlled drones to prevent them from operating in a restricted airspace.

### Weak IV (Initialization Vector)

- Weak IV attacks exploit vulnerabilities in the encryption process, particularly targeting outdated encryption protocols like WEP (Wired Equivalent Privacy).

	- Examples Include:

		- Intercepting and decrypting WEP-encrypted Wi-Fi traffic using tools like Aircrack-ng and capturing weak IVs.

		- Exploiting predictable IVs in WEP to launch attacks that reveal the network's encryption key.

### WPA3 attack

- WPA3 attacks target weaknesses or implementation flaws in the WPA3 (Wi-Fi Protected Access 3) security protocol.

	- Examples Include:

		- Exploiting vulnerabilities in the WPA3 handshake process to bypass authentication and gain unauthorized access to a secured Wi-Fi network.

		- Brute-forcing weak passwords protected by WPA3-Personal encryption to gain access to the network.

### Blue-snarfing

- Blue-snarfing involves unauthorized access to information on a Bluetooth-enabled device, such as contacts, emails, or files.

	- Examples Include:

		- Exploiting a vulnerability in a smartphone's Bluetooth implementation to remotely access its contact list and personal data.

		- Using specialized software to intercept Bluetooth communications between a mobile device and a car's infotainment system to steal sensitive information.

### Blue-jacking

- Blue-jacking is the act of sending unsolicited messages or data to Bluetooth-enabled devices within range, often for advertising or social engineering purposes.

	- Examples Include:

		- Sending anonymous messages or business cards to nearby Bluetooth-enabled smartphones in a crowded area to elicit a response or prank unsuspecting users.

		- Broadcasting promotional messages or advertisements to Bluetooth-equipped digital signage or display boards in public spaces.

### RFID (Radio Frequency Identification)

- RFID attacks target vulnerabilities in RFID systems to exploit or manipulate RFID tags or readers.

	- Examples Include:

		- Cloning RFID access cards used for building entry systems to gain unauthorized physical access to secured facilities.

		- Intercepting and modifying data transmitted between RFID tags and readers in a supply chain environment to alter inventory records or steal goods.

### NFC (Near Field Communication)

- NFC attacks exploit weaknesses in NFC-enabled devices or protocols to perform unauthorized transactions or access sensitive data.

	- Examples Include:

		- Intercepting NFC payment transactions between a smartphone and a point-of-sale terminal to capture credit card information for fraudulent purposes.

		- Exploiting vulnerabilities in NFC-enabled access control systems to bypass authentication and gain unauthorized entry to restricted areas.





# Man-in-the-Middle Attacks





## MITM


- A Man in the middle can be a good (Proxy, ALG, Translators) or it can be dangerous (Proxy ARP, DHCP Spoofing)

- A system with the ability to view the communication between two (or more) hosts (frames, packets) injects itself in the path between host systems

- They are complex attacks that ban be simplex or duplex at different layers of the OSI model.


## Man-in-the-Browser Attack

- Man-in-the-Browser attack uses the same tactics as the MITM except that a Trojan horse is used to capture and manipulate calls between the main browser and its security mechanisms (or libraries) on an ad-hoc basis. 

- The most common usage is financial fraud, which manipulates transactions of Internet banking and brokerage sites. 

- Works even when other authentication factors are being used. 





# Layer 2 Attacks





## ARP (Address Resolution Protocol) Poisoning


- A form of MITM attack that exploits ARP

- Malicious hosts inject false frames in order to corrupt (poison) the ARP cache buffers on endpoints, switches, servers, firewalls, and routers.

- Exploit kits have several scripts, modules, and tools to compromise the ARP protocol.

- It can be mitigated with port security, snooping binding databases on switches, MACsec implementation 802.1AE


## MAC Flooding


- This attack floods a switch's MAC address table with fake MAC addresses.

- It overwhelms the switch's ability to handle legitimate MAC address mappings.

- It can lead to a switch functioning as a hub, allowing attackers to intercept network traffic.


## MAC Cloning


- This involves copying the MAC address of a legitimate device onto another device.

- It allows the cloned device to impersonate the legitimate device on the network.

- Attackers can use MAC cloning to bypass MAC address-based security measures or to conduct identity theft on a network.





# DNS Attacks





## Domain Hijacking DNS Attack


- Domain hijacking or click-jacking, is also called user interface redress attack, UI redress attack, and UI redressing.

- Hacker uses several transparent layers to trick users into clicking on a button (or link) on another web page when they were actually trying to click on the top-level web page.

- Attacker hijacks clicks meant for their page and routes them to another page, often controlled by another domain or application.

- Keystrokes can also be hijacked with skillfully constructed iframes, CSS, and text boxes. 

- This can also be done through URL redirection. 


## DNS Poisoning


 - This attack involves corrupting the DNS cache with false information.

 - Attackers can manipulate DNS records to redirect users to malicious websites.

 - It can be achieved through various methods such as DNS spoofing or cache poisoning.

 - DNS poisoning can result in users unknowingly accessing fake websites or being redirected to phishing pages.


 ## Domain Reputation Attacks


 - Involves tarnishing the reputation of a domain or website to undermine trust.

 - Attackers may engage in activities like spamming or hosting malicious content to damage a domain's reputation.

 - These attacks aim to lower the credibility of the domain in the eyes of users and search engines.

 - Negative reputation can lead to reduced traffic, blacklisting by email providers, or lower search engine rankings.





 # Steps needed for a TCP Connection





1. **TCP Handshake:**

	- Initiated by the client sending a SYN (Synchronize) packet to the server.

	- Server responds with a SYN-ACK (Synchronize-Acknowledgment) packet to acknowledge the SYN.

	- Client acknowledges the server's response with an ACK (Acknowledgment) packet.

		> SYN - SYN-ACK - ACK


2. **Data Transfer:**


	- After the handshake, data transmission occurs bidirectionally between the client and server.

	- Both parties can send and receive data packets.

3. **Connection Termination:**


	- Either party can initiate the connection termination process.

	- The party initiating termination sends a FIN (Finish) packet.

	- The other party responds with an ACK packet to acknowledge the termination request.

	- Finally, the party acknowledging the termination sends its own FIN packet.

	- Upon receiving the final FIN packet, both sides complete the connection termination.





# Risk Types





## Risk Types


- Structured Threats

	- Planned

	- Organized

	- Persistent

	- Multi-phased

	- Can be external or internal

	- Exploit Kits, zero-days, modules, and ransomware

- Unstructured threats

	- Accidental

	- Non-malicious

	- Drive-by Web Surfing

	- No AUP

	- Poor awareness

	- E-mail and web-mail

	- USB's and personal electronics

- Multi-Party Risks

	- Organizations that operate with outsourcing, suppliers, licensees, agents, and the like.

	- The frequency and scale of third-party use has grown substantially over the last two decades.

	- There is greater regulatory emphasis on how organizations manage third parties to address the inherent risks

	## Internal Risks


	- Can be introduced due to the following:

		- Poor physical security

		- Lack of additional authentication Factors

		- Non-enforcement of security policy

		- Substandard auditing and monitoring of privileged insiders

		- Poor patch, configuration, and change management

		- Lack of automated vulnerability assessment

		- Absence of endpoint detection


## Risk Management Strategies 

- Risk Acceptance


	- Do not implement safeguards
		- Justification in writing is often required

- Risk Avoidance

	- Choose not to undertake actions that reduce risk

- Risk Transference/sharing

	- Pass the risk to a third-party, such as an insurance company or a cloud service provider.

- Risk mitigation

	- Implement safeguards that will eliminate or reduce risk exposure - risk may exist, but impact is reduced


## Risk Analysis


- **Defining Risk**

	- Usually described as a percentage, or probability.

		- **Inherent** (total) risk:

			- Risk the organization faces if safeguard is not implemented

		- **Residual**:

			- Risk that remains once a safeguard is in place

		- **Residual = inherent risk-safeguards (controls)**


- **Assessing Risk**

	- What are your assets at risk?

		- Both tangible and non-tangible

		- Value

	- Identify risks to those assets

		- Vulnerability, threats, and attacks

		- Who, Why, and How

	- Only focus on risks that are likely to occur

		- Maximizes available resources

		- Focus on most likely to least likely


- **Risk Register**

	- Scatter plot/table

	- Fulfills regulatory compliance

		- Repository of identified risks, impact, scenarios, and potential responses


- **Qualitative Risk Analysis**

	- Descriptive approach using subjective opinions, history, and scenarios to determine risk levels. 

		- Expert Judgement

		- Best practices

		- Experience

		- Intuition

	- Often involves interviewing people (using Delphi methods) regarding assets, known risks, known vulnerabilities, common threats, and historical impacts.

	- Impact (Magnitude) vs. Likelihood (Probability)

		- Usually measured on a scale


## Delphi Method

- The Delphi method is a structured communication technique used to gather opinions from a group of experts on a particular topic or problem. Here's how it typically works:

	- **Selection of Experts**: 

		- A panel of experts with knowledge or expertise in the relevant field is selected. These experts may come from diverse backgrounds but share a common interest in the subject matter.

	- **Anonymity**: 

		- The experts participate anonymously, which means their identities are typically concealed from each other. This anonymity encourages honest and unbiased input.

	- **Round-Based Feedback**: 

		- The process typically involves multiple rounds of questioning or surveys. In each round, experts are asked to provide their opinions, forecasts, or evaluations on specific questions or scenarios related to the topic under consideration.

	- **Feedback and Iteration**: 

		- After each round, the responses are compiled and summarized by a facilitator or moderator. The results are then shared with the experts in subsequent rounds. Experts may revise their opinions based on the feedback received from others in previous rounds.

	- **Consensus Building**: 

		- The goal of the Delphi method is often to reach a consensus or convergence of opinions among the experts. This consensus may be achieved through repeated rounds of questioning and feedback until the responses stabilize or converge around a particular viewpoint or prediction.

	- **Final Report**: 

		- Once the process is completed and consensus is reached (or a predetermined stopping point is reached), a final report summarizing the findings, insights, and consensus of the expert panel is typically generated.

- The Delphi method is commonly used in various fields such as forecasting, strategic planning, policy-making, and technology assessment, where there is uncertainty or complexity, and input from multiple experts can provide valuable insights and predictions.


## Quantitative Risk Analysis


- Scientific/mathematical approach to getting monetary and numeric results based on the following:

	- Asset values

	- Impact and magnitude

		- Severity of incident

	- Probability and likelihood of occurrence

		- Threat frequency

	- Costs and effectiveness of safeguards

	- Probabilities based on percentages and calibrated estimation


## Classic (Whitman) Quantitative Analysis


- **AV (Asset Value)**

	- Value of the asset according to the organization

- **EF (Exposure Factor)**

	- Percentage of asset loss caused by identified threat

- **SLE (Single Loss Expectancy)**

	- Potential loss of attack occurs

	- `[Asset Value] * [Exposure Factor]`

- **ARO (Annualized Rate of Occurrence)**

	- Estimated frequency the threat will occur within a single year

- **ALE (Annualized Loss Expectancy)**

	- `[SLE] * [ARO]`
	

![Whitman](https://github.com/DKC-Bluegeneral/GitBluePublic/blob/main/Images/Whitman-Tolerability-Curve.png)


## Disaster Types and Classifications

- **Environmental**

	- Earthquakes

	- Wildfires

	- Flooding

	- Snow

	- Tsunamis

	- Hurricanes

	- Tornados

	- Landslides

	- Asteroids

- **Man-Made Intentional**

	- Arson

	- Terrorist

	- Political

	- Break-Ins

	- Theft

	- Damage

	- File Destruction

	- Information Disclosure

- **Man-Made Unintentional**

	- Mistakes

	- Power Outage

	- Illness

	- Pandemics

	- Information Disclosure

	- Damage

	- File Destruction

	- Coding Errors


## Business Impact Analysis


- Risk assessment aspect of the Business Continuity Plan (BCP)

	- Identify critical functions to the business and prioritize them based on need for survival

- Identify the risks associated with the critical functions

	- The probability of risk occurring (Likelihood)

	- The impact the risk will have (Magnitude)

- Identify how to eliminate the risk or reduce the risk


## Recovery Time Objective (RTO)

- The amount of time available to recover the resource, service, or platform

	- This must be equal to or less than the Maximum Tolerable Downtime (MTD)

	- Any solutions must be accomplished within this time frame or it is considered a loss. Examples include:

		- Add physical security

		- Add redundancy

		- Purchase insurance

		- Invest in backup generators

		- Investment in faster components

		- Safeguard media off-site


## Recovery Point Objective (RPO)

- The point in time, relative to a disaster, where the recovery process begins

	- **Questions to ask yourself:**

		- How much work can be lost if a disruption occurs?

		- What impact will it have?

		- How do we make sure we don't lose more than "X" information/data?

	- This is usually your last backup, or restore point that was performed before the destructive event.


## Mean Time Between Failures (MTBF)


- A measure of how reliable a hardware system or component is
- For most devices, the measure is in thousands, or tens of thousands of hours between failures
- For example:
	- An SSD may have a mean time between failures of 10 years
		-Typically SSD's have a MTBF that is much longer than HDD's


## Mean Time to Repair (MTTR)


- How long does it take to repair?

	- Measures time it takes to fix it

	- Average value predicted based on experience and documentation. 

	- It can be calculated by:

		`[Total Down Time] * [Number of Breakdowns]`


## Maximum Tolerable Downtime

- Absolute maximum amount of time that a resource, service, or function can be unavailable before we start to experience a loss

- Factors to consider are:

	- Finances

	- Life/Safety

	- Regulatory

	- Legal/Contracts

	- Reputation

	- Property


## Privacy Breach Consequences


### Main causes of Data Breach

- **Cyber Attacks**

	- Unauthorized access or intrusion into computer systems or networks with malicious intent.

- **Device Loss or Theft**

	- Physical loss or theft of devices such as laptops, smartphones, or external drives containing sensitive data.

- **Employee Leakage or Theft**

	- Intentional or unintentional disclosure of sensitive information by employees, either through negligence or malicious intent.

- **Human Errors**

	- Mistakes or errors made by employees or system users that lead to the exposure or compromise of sensitive data.

### 6 Major Forms of Loss

- **Productivity**

	- Disruption of normal business operations and workflow, resulting in decreased productivity and efficiency.

- **Response**

	- Costs associated with incident response, including investigation, mitigation, and recovery efforts.

- **Replacement**

	- Expenses related to replacing compromised hardware, software, or infrastructure affected by the breach.

- **Fines and Judgements**

	- Financial penalties imposed by regulatory authorities or legal judgments resulting from non-compliance with data protection regulations or breach of privacy laws.

- **Competitive Advantage**

	- Loss of market position or competitive edge due to damage to brand reputation or loss of customer trust.

- **Reputation**

	- Long-term damage to the organization's reputation and trustworthiness among customers, partners, and stakeholders.


## Data Type Classifications

- **Military Classifications**

	- Top Secret

	- Secret

	- Sensitive but unclassified (SBU)

	- Confidential

	- Unclassified

- **Commercial Classifications**

	- Corporate confidential

	- Personal Confidential

	- Trade secret/Proprietary

	- Private

	- Public

	## Roles and Responsibilities

	- **Chief Privacy officer**

		- Ensures the privacy of all data in the entire organization

	- **Owner**

		- Owner of the information

		- Determines the classification level

	- **Steward**

		- Manager of the data and metadata

		- Ensures compliance (Standards/Controls) and data quality

		- Manages from a business standpoint

	- **Custodian**

		- Keeper of information

		- Ensures C.I.A. is maintained

		- Manages from a technical standpoint

	- **Processors**

		- Handles data entry and input

		- Can be an automated process or script


## Privacy Enhancing Techniques

- **Tokenization for Privacy Enhancement**

	- Data tokenization is a technique used to remove directly identifying elements

	- The process replaces the raw data with randomly generated tokens (or pseudonyms)

	- It is most often deployed with structured data, like payment cards or Social Security numbers

	- The original data does not leave the enterprise in order to meet regulatory requirements 

- **Data Minimization for Privacy**

	- A directive that states that collected and processed data should not be kept or used unless it is critical. 

	- The details should be determined early in the life-cycle to support data privacy standards such as the General Data Protection Regulation (GDPR)

	- Data that was collected for one purpose, can not be used for another purpose without consent


- **Masking and Anonymization**

	- Also known as data anonymization or pseudonymization

	- Involves stripping out or replacing any data that can identify a subject, Examples include:

		- Personally Identifiable Information (PII)

		- Protected Health Information (PHI)

		- Payment Card Information (PCI-DSS)

		- Intellectual Property (ITAR and EAR)

	- In the military this is known as "Redacting"


	## Additional Privacy Concepts


	- **Information Life Cycle**

	    - The Information Life Cycle refers to the stages through which data progresses from its creation or acquisition to its eventual disposal. These stages typically include data creation, storage, processing, transmission, and destruction. Organizations must manage data throughout its life cycle to ensure compliance with privacy regulations, maintain data integrity, and protect individuals' privacy rights. For example, data may be collected from customers during online transactions, stored in databases for analysis, transmitted to third-party service providers for processing, and eventually deleted or anonymized when no longer needed.


	- **Impact Assessment**

	    - An Impact Assessment, also known as a Privacy Impact Assessment (PIA) or Data Protection Impact Assessment (DPIA), is a systematic evaluation of the potential risks and impacts of a data processing activity on individuals' privacy and data protection rights. Impact assessments are conducted to identify and mitigate privacy risks, assess compliance with privacy regulations such as GDPR, and enhance transparency and accountability in data processing practices. For example, an organization launching a new product or service that involves the collection and processing of personal data may conduct an impact assessment to evaluate the potential privacy risks and implement appropriate safeguards to protect individuals' privacy.


	- **Terms of Agreement**

	    - Terms of Agreement, also referred to as Terms of Service (ToS) or Terms and Conditions, are legal agreements between a service provider and users that outline the terms, conditions, and rules governing the use of the service or platform. Terms of Agreement often include provisions related to data collection, processing, and sharing practices, as well as users' rights and responsibilities regarding their personal data. By accepting the terms of agreement, users consent to the service provider's data practices and agree to abide by the specified terms and conditions. For example, social media platforms typically require users to agree to their terms of service, which outline how user data will be collected, used, and shared.


	- **Privacy Notices**

	    - Privacy Notices, also known as Privacy Policies or Fair Processing Notices, are statements or documents provided by organizations to individuals that explain how their personal data is collected, processed, used, and protected. Privacy notices inform individuals about their privacy rights, the purposes for which their data is being processed, the legal basis for processing, data sharing practices, and contact information for inquiries or complaints. Organizations are required to provide clear and transparent privacy notices to individuals to ensure compliance with privacy regulations and promote transparency and trust in their data processing practices. For example, when individuals sign up for a new online service or purchase a product, they may receive a privacy notice detailing how their personal data will be handled by the organization.





# Forensics





## Incident Response Steps


- **Preparation:**

	- This phase involves establishing policies, procedures, and mechanisms to prepare for potential security incidents. It includes tasks such as creating incident response plans, defining roles and responsibilities, and implementing security controls.

- **Detection:**

	- In this phase, security teams actively monitor systems and networks for signs of security incidents. Detection mechanisms may include intrusion detection systems (IDS), security information and event management (SIEM) tools, and manual monitoring by security personnel.

- **Analysis:**

	- Once a potential security incident is detected, the next step is to analyze the nature and scope of the incident. This involves gathering evidence, conducting forensic analysis, and assessing the impact on affected systems and data.

- **Containment:**

	- After analyzing the incident, the focus shifts to containing its spread and minimizing further damage. This may involve isolating affected systems or networks, blocking malicious activity, and preventing unauthorized access.

- **Eradication:**

	- In this phase, security teams work to completely remove the threat actor from the environment. This may involve removing malware, closing security vulnerabilities, and restoring affected systems to a known good state.

- **Recovery:**

	- Once the threat has been eradicated, the final phase is to restore affected systems and operations to normal. This may involve restoring data from backups, reconfiguring systems, and implementing additional security measures to prevent future incidents.



## Acquisition of Data


- **Order of Volatility (Important):** 
	- Understanding the sequence in which volatile data should be collected to ensure its preservation before it is lost or overwritten. This hierarchy typically includes capturing system memory first, followed by network state, running processes, open files and ports, registry and temporary file systems, disk swap space, and non-volatile data from hard drives and removable media.

- **Linux `DD` Command:** 
	- A versatile tool used in Linux and Unix-like operating systems for low-level copying and conversion of data. Commonly used for disk imaging to create exact copies of storage devices or partitions, preserving not only file contents but also partition tables, boot sectors, and other metadata.

- **Data Acquisition Methods:**

  	- **Live System Imaging:**

  		- Acquiring data from a live system while it is running, often using specialized tools or techniques to minimize disruption and maintain system integrity.

  	- **Remote Acquisition:**

  		- Gathering data from a remote system or network location, typically over a network connection. Requires appropriate permissions and access controls to ensure legal and ethical compliance.

  	- **Network-Based Data Capture:**

  		- Intercepting and capturing data packets as they traverse a network, often using specialized hardware or software tools such as packet sniffers or network intrusion detection systems (NIDS).

- **Chain of Custody Documentation:**

	- Documenting the chronological history of evidence collection, handling, and transfer to establish its integrity and admissibility in legal proceedings. Includes details such as who collected the evidence, when and where it was collected, and any changes in possession or custody.

- **Hashing Techniques for Data Integrity Verification:**

	- Using cryptographic hash functions to generate unique identifiers (hash values) for data sets, allowing verification of data integrity by comparing hash values before and after acquisition. Common hashing algorithms include MD5, SHA-1, and SHA-256.

- **Legal Considerations and Compliance Requirements:**
	- Understanding the legal and regulatory frameworks governing data acquisition and forensic investigations, including privacy laws, chain of custody requirements, and rules of evidence. Compliance with industry standards and organizational policies is also essential.

- **Data Recovery Techniques:**

	- Methods and tools used to recover data from damaged or corrupted storage devices, including hard drives, solid-state drives (SSDs), and removable media. Techniques may include file system repair, sector-by-sector imaging, and specialized data recovery software.

- **RAM Acquisition Tools and Methods:**

	- Tools and techniques for capturing volatile data from system memory (RAM) during live forensics investigations. This may involve using dedicated hardware devices, software utilities, or forensic analysis frameworks to acquire and analyze RAM contents.

- **Write Blocking Mechanisms:**

	- Hardware or software-based mechanisms used to prevent accidental or unauthorized write operations to storage devices during data acquisition. Write blockers ensure data preservation and maintain evidentiary integrity by preventing alterations to original data.

- **Metadata Preservation Techniques:**

	- Preserving metadata associated with digital evidence, including file attributes, timestamps, and file system metadata. This information can provide valuable context and provenance for forensic analysis and legal proceedings.



## Preservation of Data


- **Use a Write Blocker:**

	- Employing hardware or software-based write blockers to prevent any modification or alteration of data during the preservation process. Write blockers ensure the integrity of original evidence by blocking write operations to storage devices, thus preserving the data in its original state.

- **Hashing for Verification:**

	- Generating hash values of preserved data to verify its integrity and authenticity. Hashing algorithms such as MD5, SHA-1, and SHA-256 can be used to create unique fingerprints of data, allowing comparison before and after preservation to ensure no tampering has occurred.

- **Chain of Custody Documentation:**

	- Documenting the handling and transfer of preserved data to establish its integrity and admissibility in legal proceedings. Chain of custody logs should include details such as who collected the data, when and where it was collected, and any changes in possession or custody.

- **Storage in Secure Environment:**

	- Storing preserved data in a secure environment with controlled access to prevent unauthorized tampering or access. This may involve using encrypted storage devices, access controls, and physical security measures to safeguard the integrity of the data.

- **Backup and Redundancy:**

	- Creating backups of preserved data to mitigate the risk of data loss due to hardware failure, corruption, or other unforeseen events. Redundant copies of preserved data should be stored in separate locations to ensure availability and resilience against disasters.

- **Documentation of Preservation Methods:**

	- Documenting the preservation methods and techniques used to maintain the integrity of data throughout the preservation process. This documentation should include details of the tools, procedures, and safeguards employed to ensure the reliability of preserved data.

- **Legal and Regulatory Compliance:** 

	- Ensuring that preservation practices comply with relevant legal and regulatory requirements, including privacy laws, chain of custody standards, and rules of evidence. Adhering to industry best practices and organizational policies is essential to maintaining the defensibility of preserved data in legal proceedings.

- **Periodic Integrity Checks:**

	- Conducting periodic integrity checks on preserved data to verify its continued integrity and detect any signs of tampering or corruption. This may involve re-hashing data, comparing checksums, or using digital forensic techniques to validate the authenticity of preserved evidence.



## Reporting


- **Types of Reports:**

	- Different types of reports serve various purposes in cybersecurity management and compliance. Incident reports document security incidents and their resolutions, vulnerability assessment reports provide insights into system weaknesses, compliance reports demonstrate adherence to regulatory standards, and executive summaries offer high-level overviews for decision-makers.

- **Incident Reporting Procedures:**

	- Establishing clear incident reporting procedures ensures that security incidents are promptly identified, reported, and addressed. This includes defining reporting channels, outlining incident classification criteria, and specifying response timeframes to minimize the impact of security breaches.

- **Reporting Tools and Software:**

	- Utilizing specialized tools and software enhances the efficiency and effectiveness of security reporting activities. SIEM systems aggregate and correlate security events from multiple sources, log management platforms centralize log data for analysis, and reporting modules within cybersecurity solutions generate customizable reports tailored to specific requirements.

- **Compliance Reporting Requirements:**

	- Compliance reporting is essential for demonstrating adherence to regulatory standards and industry best practices. Organizations must maintain accurate records and documentation to fulfill reporting obligations and demonstrate compliance with applicable laws and regulations.

- **Security Metrics and Key Performance Indicators (KPIs):**

	- Metrics and KPIs provide quantifiable measures of cybersecurity performance and effectiveness. Monitoring key indicators allows organizations to track progress, identify trends, and make informed decisions to improve security posture and mitigate risks.

- **Executive Reporting:**

	- Executive reports distill complex security data into concise summaries tailored to the needs of executive stakeholders. These reports highlight significant security risks, compliance issues, and strategic priorities, enabling informed decision-making at the highest levels of the organization.

- **Data Visualization Techniques:**

	- Data visualization enhances the readability and interpretability of security reports by presenting information in visual formats. Charts, graphs, and dashboards transform raw data into meaningful insights, enabling stakeholders to quickly grasp trends, patterns, and anomalies.

- **Continuous Improvement and Feedback:**

	- Continuous improvement fosters the evolution of reporting processes and practices to meet changing organizational needs and industry trends. Soliciting feedback from stakeholders promotes collaboration and ensures that reporting mechanisms remain relevant, accurate, and actionable over time.

- **Documentation and Record Keeping:**

	- Documentation and record-keeping are critical for maintaining an audit trail of security activities and decisions. Detailed records support accountability, facilitate compliance reporting, and provide evidence for audits, investigations, and legal proceedings.

- **Training and Awareness Programs:**

	- Training and awareness programs educate employees on their roles and responsibilities in reporting security incidents and maintaining data confidentiality. By promoting a culture of vigilance and accountability, organizations empower employees to proactively identify and report security threats, contributing to overall cybersecurity resilience.



## Data Sources, Dashboards, and Reports


- **Types of Data Sources:**

	- Understand the various types of data sources commonly used in cybersecurity, including logs from network devices (e.g., firewalls, routers), endpoint logs (e.g., antivirus logs, system logs), cloud service logs, application logs, and external threat intelligence feeds. Different data sources provide unique insights into security events and threats, enabling comprehensive threat detection and analysis.

- **Components of Dashboards:**

	- Dashboards are interactive visual interfaces that display key metrics, KPIs, and insights from data sources. Components of dashboards may include charts, graphs, tables, heatmaps, gauges, and widgets. Dashboards allow users to monitor security posture, track performance metrics, and identify trends or anomalies in real-time, facilitating informed decision-making and situational awareness.

- **Types of Reports:**

	- Reports in cybersecurity serve various purposes, such as incident reporting, compliance reporting, executive reporting, and trend analysis. Incident reports document security incidents and their resolutions, compliance reports demonstrate adherence to regulatory standards, executive reports provide high-level overviews for decision-makers, and trend analysis reports identify patterns and emerging threats based on historical data.

- **Data Visualization Techniques:**

	- Data visualization techniques enhance the readability and interpretability of reports and dashboards by presenting data in visual formats. Common data visualization techniques include charts (e.g., bar charts, line charts, pie charts), graphs (e.g., network graphs, tree maps), heatmaps, histograms, scatter plots, and infographics. Visualization techniques help stakeholders quickly grasp complex information, identify patterns, and derive insights from data.

- **Importance of Data Integrity:**

	- Data integrity is essential for ensuring the accuracy, reliability, and trustworthiness of reports and dashboards. Maintaining data integrity involves verifying the completeness, consistency, and correctness of data across its lifecycle. Measures to preserve data integrity include implementing access controls, encryption, data validation checks, audit trails, and data quality assurance processes. Upholding data integrity enhances the credibility of reports and dashboards, supporting informed decision-making and effective cybersecurity operations.




## Metadata

- **Definition and Types:**


	- Metadata refers to data that provides information about other data. It includes descriptive attributes that characterize the content, context, structure, and usage of data. Types of metadata commonly encountered in cybersecurity include technical metadata (e.g., file format, data size), descriptive metadata (e.g., file name, author), administrative metadata (e.g., access permissions, creation date), and structural metadata (e.g., data relationships, file hierarchy).

- **Importance in Cybersecurity:**

	- Metadata plays a crucial role in cybersecurity for various purposes, such as data classification, data management, information retrieval, forensic analysis, and compliance auditing. By providing contextual information about data assets, metadata enhances data visibility, governance, and protection, enabling organizations to better understand, manage, and secure their digital assets.

- **Examples of Metadata:**

	- Examples of metadata include file attributes (e.g., file name, file type, file size), document properties (e.g., author, creation date, modification date), network packet headers (e.g., source IP address, destination IP address, protocol type), email headers (e.g., sender address, recipient address, subject line), and database schema information (e.g., table names, column names, data types).

- **Risks and Challenges:**

	- Despite its utility, metadata can pose risks and challenges in cybersecurity, such as privacy concerns, data leakage, metadata poisoning, and metadata extraction attacks. Inadequate metadata management practices may result in unauthorized access, data breaches, and regulatory compliance violations. Organizations must address these risks by implementing robust metadata governance frameworks and security controls.

- **Metadata Management Best Practices:**

	- Effective metadata management practices are essential for maximizing the benefits of metadata while mitigating associated risks. Best practices include implementing metadata standards and schemas, establishing metadata repositories and catalogs, enforcing metadata quality controls, documenting metadata lineage and provenance, and integrating metadata management into broader data governance and security frameworks.



## Security Information and Event Management


- **Agent-based:**

	- Agent-based SIEM systems deploy software agents on individual devices or endpoints to collect and send security event data to a centralized SIEM server for analysis and correlation. These agents monitor local logs, network traffic, and system activity, providing real-time visibility into security events and threats at the endpoint level. Agent-based deployment offers granular visibility and control but may incur performance overhead and management complexity.

- **Agentless:**

	- Agentless SIEM systems leverage network-based sensors or log collectors to gather security event data from devices and network infrastructure without installing agents on individual endpoints. These sensors passively monitor network traffic, log files, and system events, extracting relevant data for analysis and correlation. Agentless deployment reduces overhead and simplifies management but may provide less visibility into endpoint activity compared to agent-based approaches.

- **Centralized Logging:**

	- Centralized logging is a fundamental component of SIEM systems, enabling the collection, storage, and analysis of security event data from diverse sources across an organization's IT infrastructure. Centralized logging consolidates log data from endpoints, servers, applications, network devices, and cloud services into a unified repository, facilitating centralized monitoring, analysis, and reporting for security operations.

- **Log Aggregation:**

	- Log aggregation involves collecting and combining log data from multiple sources into a single repository for analysis and correlation. SIEM platforms use log aggregation techniques to aggregate logs from diverse sources, normalize log formats, and enrich log data with contextual information for effective threat detection and incident response. Log aggregation enhances visibility and simplifies analysis by providing a unified view of security events and activities.

- **Correlation Rules:**

	- Correlation rules are predefined logic or algorithms used by SIEM systems to identify patterns, trends, and relationships among security events and alerts. These rules analyze event data in real-time or near-real-time, comparing events against established criteria to detect suspicious or anomalous behavior indicative of security threats. Correlation rules help prioritize alerts, reduce false positives, and automate incident response processes.

- **Alerting and Notification:**

	- SIEM systems generate alerts and notifications to notify security personnel of detected security incidents, anomalies, or policy violations. Alerts may be triggered based on predefined correlation rules, thresholds, or manual configuration settings. SIEM platforms support various alerting mechanisms, such as email notifications, SMS alerts, dashboard alerts, and integration with ticketing systems or incident response platforms.

- **Incident Response Integration:**

	- SIEM systems integrate with incident response workflows and processes to facilitate timely detection, investigation, and response to security incidents. Integration with incident response tools, ticketing systems, and workflow orchestration platforms enables seamless coordination and collaboration among security teams, streamlining incident triage, analysis, and remediation efforts.



## Alert Tuning


- **Techniques for Tuning:**

	- **Muting:**

		- Muting involves temporarily suppressing or silencing alerts for specific events or conditions that are known to be benign or expected behavior. By muting non-critical alerts, security teams can reduce alert fatigue and focus their attention on more significant security events and threats.
  
	- **Redirecting "Floods":** 

		- Redirecting floods refers to redirecting or consolidating alerts generated from a high volume of similar events within a short period. Instead of generating separate alerts for each instance of the same event, security teams can aggregate these alerts into a single notification or summary, reducing noise and improving efficiency in alert management.
  
	- **Threshold Adjustment:** 

		- Threshold adjustment involves fine-tuning alert thresholds and criteria to better align with the organization's risk tolerance and operational needs. By adjusting thresholds for event severity, frequency, or other parameters, security teams can tailor alerting rules to prioritize high-impact events while minimizing false positives and noise.
  
	- **Whitelisting/Blacklisting:** 

		- Whitelisting and blacklisting are techniques used to selectively enable or disable alerts based on predefined criteria or lists. Whitelisting allows security teams to specify trusted entities, behaviors, or conditions that should not trigger alerts, while blacklisting identifies known malicious or unwanted activities that should be flagged for further investigation. These techniques help customize alerting rules to reflect the organization's security policies and priorities.

- **Importance of Alert Tuning:** 

	- Alert tuning is crucial for optimizing the effectiveness and efficiency of security monitoring and incident response processes. By fine-tuning alerting rules and thresholds, organizations can reduce alert fatigue, prioritize high-impact events, and improve the accuracy of threat detection and response.

- **Challenges in Alert Tuning:** 

	- Alert tuning presents several challenges, including the risk of overlooking critical alerts, the complexity of managing a large volume of alerts, and the difficulty of balancing sensitivity and specificity in alerting rules. Additionally, changing threat landscapes, evolving business requirements, and technology complexities can further complicate the alert tuning process.

- **Best Practices for Effective Alert Tuning:** 

	- Effective alert tuning requires a systematic approach and adherence to best practices. Key practices include regularly reviewing and updating alerting rules, leveraging automation and machine learning techniques for intelligent alert triage, collaborating with stakeholders to understand business priorities and risk tolerances, and continuously monitoring and refining alerting processes based on feedback and lessons learned.

- **Continuous Monitoring and Review:** 

	- Alert tuning is an ongoing process that requires continuous monitoring and review to adapt to evolving threats, technologies, and business needs. Security teams should establish regular cadences for reviewing alerting rules, thresholds, and performance metrics, ensuring that alerting processes remain effective, efficient, and aligned with organizational objectives.


## Monitoring Infrastructure


- **Network Monitors:** 

	- Network monitors are tools or systems used to monitor network traffic and devices for performance, availability, and security issues. These tools capture and analyze network packets, monitor bandwidth utilization, detect network anomalies, and provide visibility into network infrastructure components such as routers, switches, firewalls, and servers.

- **Appliance State Data:** 
	- Appliance state data refers to information about the operational status and health of network appliances and devices. This data includes metrics such as CPU utilization, memory usage, disk space, interface status, and system uptime. Monitoring appliance state data helps ensure the reliability, performance, and availability of network infrastructure components.

- **Simple Network Management Protocol (SNMP) Traps:** 

	- SNMP traps are asynchronous notifications sent by network devices to a central management system (SNMP manager) to alert administrators of significant events or conditions. Traps provide real-time alerts for events such as device reboots, interface status changes, error conditions, and security breaches. SNMP traps enable proactive monitoring and troubleshooting of network devices.

- **Netflow/IPFIX (Internet Protocol Flow Information Export):** 

	- Netflow and IPFIX are protocols used for collecting and exporting flow data from network devices for traffic analysis and monitoring. These protocols capture information about network flows, including source and destination IP addresses, ports, protocols, and packet counts. Netflow and IPFIX data provide insights into network traffic patterns, application usage, and security threats.

- **Cloud Service Health:** 

	- Monitoring cloud service health involves tracking the performance, availability, and reliability of cloud-based services and resources. Cloud service providers typically offer monitoring tools and dashboards to monitor service health indicators such as uptime, latency, response times, and service-level agreements (SLAs). Monitoring cloud service health ensures optimal performance and user experience for cloud-based applications and services.

- **Syslog Servers:** 

	- Syslog servers are centralized log management systems used to collect, store, and analyze log data from network devices, servers, applications, and security appliances. Syslog servers receive syslog messages generated by network devices and servers, providing a consolidated view of system and network events. Monitoring syslog data helps identify security incidents, troubleshoot performance issues, and ensure compliance with logging requirements.



## Benchmarks


- **Scanning for Configuration Vulnerabilities:** 

	- Benchmarks involve scanning systems and networks for configuration vulnerabilities, which are weaknesses resulting from misconfigurations or deviations from secure configuration baselines. Configuration vulnerability scanning tools identify insecure settings, outdated software versions, and misconfigured access controls that could expose systems to security risks.

- **Lack of Controls:**

	- Benchmarks assess the presence or absence of security controls implemented to mitigate risks and protect systems and networks. Security controls include preventive, detective, and corrective measures such as firewalls, intrusion detection systems (IDS), access controls, encryption, and security policies. Identifying gaps or deficiencies in security controls helps prioritize remediation efforts and strengthen overall security posture.

- **Improper Configuration:** 

	- Benchmarks evaluate the correctness and effectiveness of system configurations in aligning with security best practices and standards. Improper configurations may include default settings, unnecessary services or protocols enabled, weak authentication mechanisms, and misconfigured access permissions. Addressing improper configurations reduces the attack surface and minimizes the likelihood of successful exploitation by threat actors.

- **Security Content Automation Protocol (SCAP):**

	- SCAP is a standardized protocol developed by the National Institute of Standards and Technology (NIST) for automating security compliance assessment, measurement, and reporting. SCAP enables organizations to streamline vulnerability assessment, configuration management, and security policy enforcement across heterogeneous IT environments. SCAP-compliant tools use standardized data formats and protocols to exchange security-related information and automate security tasks.

- **Language to Enable Scanners to Load Configuration Benchmarks and Scan for Deviations:**

	- Benchmarks utilize a language or format that enables security scanners to load configuration benchmarks and compare system configurations against predefined standards or benchmarks. This language allows scanners to identify deviations or non-compliant settings and generate reports detailing security posture and compliance status. Examples of benchmark formats include Extensible Configuration Checklist Description Format (XCCDF) and Open Vulnerability and Assessment Language (OVAL).




## Malware Classification


- **Viruses:**

	- Spread within code without authorization.

- **Worms:**

	- Self-replicating malware that spreads across networks.

- **Trojans:**

	- Malicious programs disguised as legitimate software.

- **Potentially Unwanted Programs (PUPs):**

	- Software that may be unwanted or harmful, but not necessarily classified as malware.

- **Pre-installed Bloatware:**

	- Software pre-installed on devices by manufacturers, often unnecessary and resource-intensive.

- **Grayware:**

	- Software that exhibits behaviors similar to both legitimate software and malware, such as adware or spyware.

- **Classification by Payload:**

	- Categorization based on the type of malicious activity or impact, such as ransomware, spyware, or keyloggers.

- **Tracking Cookies:**

	- Cookies used to track user activity online, often for targeted advertising purposes.

- **Adware:**

	- Software that displays unwanted advertisements to users, often bundled with other software.

- **Spyware:**

	- Malware designed to secretly monitor and gather information about a user's activities.

- **Keylogger:**

	- Malware that records keystrokes typed by a user, often used to capture sensitive information such as passwords or credit card numbers.



## Backdoors and Remote Access Trojans (RAT)

- **Backdoor Malware:**

	- Backdoor malware is a type of malicious software that enables unauthorized access to a system or network by creating a hidden entry point, known as a backdoor. Attackers exploit backdoors to bypass security controls and gain persistent access to compromised systems, allowing them to steal data, install additional malware, or launch further attacks.

- **Remote Access Trojans (RAT):**

	- Remote Access Trojans (RATs) are malicious programs that provide attackers with unauthorized remote access to infected systems. RATs typically include features for remote control, file manipulation, screen capture, and keystroke logging, allowing attackers to monitor user activity, steal sensitive information, and execute commands remotely without the user's knowledge.

- **Bots and Botnets:**

	- Bots are compromised computers or devices infected with malware that allows them to be controlled remotely by a bot-master. Botnets are networks of interconnected bots that can be harnessed by attackers to perform coordinated attacks, such as distributed denial-of-service (DDoS) attacks, spam campaigns, or credential stuffing attacks. Botnets are often used to propagate malware, steal data, or carry out large-scale cyber-crime operations.

- **Command and Control (C2 or C&C):**

	- Command and control (C2 or C&C) refers to the communication infrastructure used by attackers to remotely control and manage compromised systems or botnets. C2 servers act as centralized command hubs for issuing instructions to infected devices, receiving stolen data, and coordinating malicious activities. Detecting and disrupting C2 communications is essential for mitigating the impact of malware infections and preventing further compromise.

- **Backdoors Installed Through Misconfiguration:**

	- Backdoors can also be inadvertently created through misconfigurations or vulnerabilities in software, services, or devices. Attackers exploit misconfigurations to establish unauthorized access points, bypassing authentication mechanisms and security controls. Common misconfigurations that lead to backdoor installations include default passwords, open ports, insecure network services, and un-patched software vulnerabilities.



## Rootkits

- **Local Administrator vs SYSTEM/Root Privileges:**

	- Local administrator privileges refer to the highest level of access rights granted to a user account on a local system. Users with local administrator privileges have full control over system resources and can install software, modify system settings, and access sensitive data.
	- SYSTEM or root privileges, on the other hand, represent the highest level of access rights on a computer system, typically associated with the operating system's kernel or core processes. Users with SYSTEM/root privileges have unrestricted access to all system resources and can perform privileged operations that are not available to regular users or even local administrators.
	- Rootkits are malicious software components designed to exploit vulnerabilities and gain unauthorized access to a system, often by escalating privileges to the SYSTEM or root level. Once installed, rootkits can conceal their presence, manipulate system behavior, and evade detection by security software, making them particularly dangerous and difficult to detect and remove.

- **Persistence Mechanisms:**

	- Rootkits employ various persistence mechanisms to maintain their presence on a compromised system even after reboots or security measures are applied. Persistence mechanisms may include modifying system files, registry entries, boot sectors, or system configurations to ensure the rootkit's persistence and resilience against removal attempts.

- **Kernel Level Rootkits:**

	- Kernel-level rootkits operate at the lowest level of the operating system, directly interacting with the kernel and system processes. These rootkits manipulate kernel data structures, system calls, and memory allocations to conceal their presence and control system behavior. Kernel-level rootkits are highly sophisticated and difficult to detect due to their deep integration into the operating system.

- **User Level Rootkits:**

	- User-level rootkits operate within user-space processes and applications, exploiting vulnerabilities in user-mode components to gain elevated privileges and execute malicious activities. Unlike kernel-level rootkits, user-level rootkits do not directly modify system components or kernel data structures, making them less stealthy but still effective at evading detection and performing unauthorized actions.

- **Memory Resident Rootkits:**

	- Memory-resident rootkits reside entirely in system memory, without leaving traces on disk or modifying system files. These rootkits inject malicious code into running processes or system memory regions, allowing them to intercept system calls, manipulate system behavior, and hide their presence from traditional file-based security tools. Memory-resident rootkits are difficult to detect and remove due to their volatile nature and ability to evade disk-based scanning techniques.

- **File System Rootkits:**

	- File system rootkits manipulate file system structures and objects to conceal their presence and control system behavior. These rootkits may modify file attributes, directory entries, or file contents to hide malicious files, processes, or network connections from users and security tools. File system rootkits can be persistent or non-persistent, depending on their ability to survive system reboots and security measures.

- **Detection and Removal Techniques:**

	- Detecting and removing rootkits require specialized tools and techniques capable of identifying stealthy and persistent malware components. Detection techniques may include memory forensics, system integrity checks, behavioral analysis, and heuristic scanning. Removal techniques may involve using rootkit-specific removal tools, bootable antivirus rescue disks, or performing system restores from clean backup images.



## Ransomware 

- **Definition and Characteristics:**

	- Ransomware is a type of malicious software designed to encrypt files or block access to a computer system or data until a ransom is paid. It typically exhibits characteristics such as file encryption, ransom demands, payment instructions, and deadlines for payment. Ransomware may also display threatening messages or warnings to coerce victims into paying the ransom.

- **Encryption Techniques:**

	- Ransomware employs advanced encryption techniques, such as symmetric or asymmetric encryption algorithms, to encrypt files and data on infected systems. Symmetric encryption uses a single encryption key to encrypt and decrypt data, while asymmetric encryption uses a pair of public and private keys for encryption and decryption. Encryption keys are generated by the ransomware and stored on remote servers controlled by the attackers.

- **Delivery Methods:**

	- Ransomware can be delivered to victims through various attack vectors, including malicious email attachments, phishing links, exploit kits, malicious websites, removable media, and compromised software or applications. Attackers may also leverage social engineering tactics to trick users into downloading and executing ransomware payloads.

- **Ransom Payment and Cryptocurrency:**

	- Ransomware typically demands payment in cryptocurrency, such as Bitcoin, Ethereum, or Monero, to facilitate anonymous transactions and evade law enforcement detection. Victims are instructed to purchase cryptocurrency and transfer the ransom amount to a specified wallet address controlled by the attackers. Payment does not guarantee decryption or restoration of data, as attackers may fail to provide decryption keys or tools after receiving payment.

- **Impact on Organizations:**

	- Ransomware attacks can have devastating consequences for organizations, including data loss, financial losses, operational disruptions, reputational damage, and regulatory penalties. Ransomware infections may result in encrypted files, system downtime, loss of productivity, customer trust erosion, and legal liabilities, posing significant risks to business continuity and information security.

- **Mitigation Strategies:**

	- Organizations can implement various mitigation strategies to prevent, detect, and respond to ransomware attacks. These strategies may include regular data backups and offsite storage, employee security awareness training, patch management, endpoint protection solutions, network segmentation, email filtering, incident response planning, and ransomware-specific security controls.

- **Incident Response and Recovery Procedures:**

	- Effective incident response and recovery procedures are essential for minimizing the impact of ransomware attacks and restoring affected systems and data. Organizations should have incident response plans in place to guide response efforts, including containment, eradication, recovery, and communication with stakeholders. Recovery procedures may involve restoring data from backups, decrypting files using decryption tools or services, and rebuilding compromised systems from clean images.

 












































## Random

- Do day 7 lab for log files
- Get your SIEM up and running and learn to read logs and packets.

