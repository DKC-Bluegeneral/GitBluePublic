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





-------------------------------------------------------------Add Previous notes above this text------------------------------------------------------------------------------------------





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
	- Environmental attributes (time fo access, location, etc.).

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

- SUID (Set User ID [SUDO]) It is a special permission in Unix-like operating systems that allows users to execute a file with the permissions of the file's owner or group, rather than with the permissions of the user who is executing it.





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


## Injection Attacks


- Often a result of MITM (Man in the middle) or RAT (Remote Access Tool).

- Malware can inject false MAC or IP addresses.

- DLL injection is where malicious code forces itsself to rin in place of other benign code.

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

- XML metacharacters can be used to modify

- Can interfere with application logic

- Performs unauthorized tasks or accessable data. 


## Coding Attacks


- **Pointer/object dereference**

	- An attacker can supply a pointer for memory locations that the program is not expecting

	- A Null-pointer dereference occurs when a pointer with a value of NULL is used as if it actually points to a valid memory area

	- A program can possibly dereference a null pointer, and in doing so, raise a NullPointerException

	- Null pointer errors are frequently the result of one or more programmer assumptions being violated. 

- **Directory Traversal**

	- Also known as a path transversal attack or a "Dot Slash" and is most often launched through a web browser and other clients.

	- This HTTP exploit allows and attacker to access restricted files, directories, and commands located outside of the root directory

	- Attackers can modify a URI or URL to force the web server into exposing the restricted files.

		- Examples Include:

			![Example 1](https://raw.githubusercontent.com/DKC-Bluegeneral/Notes/main/Images/Dir-Transversal-Example-1.png)


## Buffer and Integer overflows


- **Buffer Overflows**

	- Attacker Sends larger than expected input, for example when a server accepts it and writes to memory areas.

	- Associated buffers are filled and adjacent memory is overwritten as a result.

	- This everwrite may contain instructions or code that crashes the server resulting in a DoS.

- **Integer Overflows**

		- A Type of an arthmetic overflow error when the result of an integer operation does not fit  within the allocated memory space.

		- Instead of an error in the program, it usually causes the result to be unexpected.

		- These are in the top 10 of the most dangerous software errors, mostly because they often lead to buffer overflows.

- Race Conditions - time of check/time of use

	- **Race Condition**

		- A race condition is when a system or software trise to do two or more things simultaneously, but due to the type of system, the operations must be done in the correct sequence in order or function properly.

		- Race conditions are classically related to synchronization errors in software code.

		- Crackers can leverage a known race condition vulnerability to get unauthorized access to a system or network.

	- **Time-Of-Check vs. Time-Of-Use (TOC/TOU)**

		- A time-of-check vs time-of-use attack is a race condition and occurs when an attacker tries to gain privelege to a system by "racing" it to a resource it is attempting to access.

		- The types of programming flaws that allow for race conditions occur when the system (or application) splits up the operations of verifying credentials and providing access to a resource.

		- It can do things such as replacing a config.sys file with a different file that compromises the system before the system even loads it's operating system.

- Improper error handling

	- Poorly defined validation rules used in verifying the correctness, completeness, and acceptability of input data.

	- Software applications and web servers are notorious

	- Must establish data input, data flow, and data output requirements with a designed security features in mind.

	- Collusions are in this category when the chance that two unique inputs will produce the same output (MD5 and SHA-1 are vulnerable)

- Session replay attacks

	- Often part of MITM attacks.

		- Examples include:

			- An attacker steals an ID of a user and reuses it to impersonate an authorized user.

			- Web applications that allow reusing old session ID's or session credentials for authorization are also vulnerable to these attacks.

	- IPsec (Internet Protocol Security) and TLS (Transport Layer Security) have anti-replay mechanisms to protect secure session.





# API Attacks




- Application Programming Interface Attacks:

	- An API DDoS attack often involces sending traffic from many clients to overwhelm the API service

	- Even if rate limiting controls are in place to prevent servers from crashing, they cannon always prevent service disruption and severe degradation of the API's user expierence.

	- If API calls are not digitally signed or if they have embeded credentials, they can be compromised.


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

	- On Windows networks, hackers do not need the plaintext passwords to access certian services.

	- Sometimes the authentication process relies on the passwords cryptographic hash and there are various tools to extract these hashes (Cain) from compromised Windows machines (Lately Windows 10) and use them to access other services.

	- This technique is known as pass the hash and is one of the attacks that windows Virtual Secure Module (VSM) was intended to protect against.

- By definition a Pass the Hash is a vulnerability of Windows Safe Mode.

	- It is an OS diagnostic mode of peration that has been around since windows 95

	- It can be initiated at the boot time and only loads the nominal set of drivers and services that windows needs to run.

	- Most third-party security products do not start up in safe mode so the protection is negated.






# Driver Manipulation





- A Common vector is the hardware drivers that we install in our operating systems

- This is priveleged code that is trusted by the OS

- Can be trojans, RATs, or hacked driver software


## Shimming


- Shimming is the process of stealing information and money from Point-of-Sale (POS) systems, credit card readers, and ATM machines.

- The attack is common at gas stations, convienence stores, and kiosks.

- It can be an overlay attachment or sometimes and entirely replaced device.

	![Example2](https://github.com/DKC-Bluegeneral/Notes/blob/main/Images/ATM-Skimmer-Example-2.png)


## Refactoring

- Involves changing an applications source code without modifying the characteristics.

	- Often used to introduce legacy applications into new computer systems and devices. 

	- Can also re-engineer classic attack code to create variants, hybrid viruses, and worms. 




# Wireless Attacks





## Common Wireless Attacks


- Most malware attacks are multi-phased, stealthy, and polymorphic. Below is a list of some common wireless attacks:


	- Evil Twins
	- Rogue AP
	- Disassociation
	- Jamming
	- Weak IV
	- WPA3 attack
	- Bluesnarfing
	- Bluejacking
	- RFID
	- NFC