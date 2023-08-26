# Introduction to Cybersecurity
### 3 Principles of Cybersecurity:
**CIA triad**
1.	**Confidentiality (机密性):**
Make sure the data is kept safe and only the authorized person can access.
2.	**Integrity （完整性）:**
The data is authentic and not tempered with. Ensure data not alter through hash. 
3.	**Availability （可用性）:**
Users or organizations can access the networks, servers, and applications at anytime and anywhere. Always to make sure to have backups.

**Opposite of CIA : DAD (Disclosure, Alteration, Deny)**
1. **Disclosure** – confidentiality had been compromised
2. **Alteration** – data had been compromised, modified
3. **Destruction/Deny** – server shutdown, disruption, server does not respond

### Cybersecurity Framework
1.	**Identify (ID)**: identify management; notification from detection system is investigated.
2.	**Protect (PR)**: develop and implement appropriate safeguards to ensure identity assets management.
Cyber security training for employees; creating and monitoring baseline.
3.	**Detect (DE)**: develop and implement appropriate activities to identify the occurrence of a cybersecurity event. 
Detection processing; machine leaning; real-time monitoring.
4.	**Respond (RS)**: take actions regarding a detected cybersecurity incident respond planning.
Communication, Analysis, Mitigation, Improvement, Achieve history logs.
5.	**Recover (RC)**: maintain plans. 
Recover planning, get OP back online, version control.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**“You can’t secure what you don’t know!”**_

### Security Controls:
1.	**Physical controls**: physical hardware device, such as badge reader, lock
2.	**Technical controls**
3.	**Administrative controls:** guidelines or advisories aimed for employees.

**ISO Design Principles:**
1. L**east Privilege:** access given according to user’s position/jobs functions
2. **Attack surface minimisation:**  Example : closing the ports those are expose to public
3. **centralized parameter** : to prevent SQL injection 
4. **Services** : ratio server, firewall. 
5. **Preparing for Error and exception handling** : SQL injection practice 

### Access Control Concept
A subject: any entity that requests access to our access. Example: user, client, process or program, device endpoint.
An object: anything that a subject attempts to access; responds to a request for service. Example: building, computer, a file, printer or scanner, server, database, software, task, thread or process.
Rules: Access rule is an instruction developed to allow or deny access to an object by comparting the validated identity of the subject to an access control list. Example: Firewall
1.	**Defense in Depth**
Layered defense where a data center contains: Physical controls, Logical/Technical controls, administrative controls, Assets.
2.	**Principle if Least Privilege**
A standard of permitting only minimum access necessary for users or programs to fulfill their functions.
3.	**Privileged Access Management**
Granted various create, read, update, delete privileges on database.
4.	**Privileged Accounts**
Those with permissions beyond those of normal users, such as managers and administrators.

### SIEM (Security Information and Event Management)
* To detect security threats
* Real times logging events in own environments
* Examples: Splunk, IBM, QRadar, ArcSight ESM, FortiSIEM

### SOAR (Security Orchestration Automation and Response)
* Network. Threat Intelligence, Mobile, Endpoints, Identify & Access, Cloud Security, WAF & App Security, Web Proxy & Firewall.
* Examples: Splunk Phantom, IBM Resilient, Logsign, Demisto

### EDR (Endpoint Detection and Response)
* CarbonBlack, SentineOne, FireEye HX

### 5 stages of Penetration Test:
_**Must have permission before to attack machine/network!**_
1.	**Reconnaissance/Information Gathering</br>**
Actively - social engineering</br>
Getting IP address:</br>
- ping address.com
- nslookup webaddress
- whois webaddress.com
Passively – Google</br>
2.	**Scanning**: find opening gateways/ports</br>
_**Scanning is not allow to without permission from the target!!**_
-	whatweb webaddress</br>
level of aggression : 1) stealth for public request 3&4) for penetration testing only
3.  **Gaining Access/Exploitation**: hack
4.	**Maintaining Access**: planning back door, root kits
5.	**Covering tracks**: remove tracks by removing files, edit logs, etc.
