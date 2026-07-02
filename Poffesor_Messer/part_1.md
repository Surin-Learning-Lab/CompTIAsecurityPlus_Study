# ***1.1 Security Controls***

**Technical Controls**  
-controls implementation using systems  
-Operating system controls  
-firewalls, anti-virus  

**managerial Controls**  
-Administrative controls associated with security design and implementation  
-Security polices, standard operating procedures, creating security polices and documentation  

**Operational Controls**  
-Controls implemented by people instead of systems  
-Security guards, awareness programs  

**Physical Controls**  
-Limit physical access  
-guard shack  
-fences, locks  
-badge readers  



***Control type categories***  

**Preventative control types**  
-block access to a resource  

-firewall rules *(technical)*  
-follow security policy *(managerial)*  
-Guard shack checks all identification *(operational)*  
-enable door locks *(physical)*  

**Deterrent control types**  
-discourage an intrusion attempt  
-does not directly prevent access  

-application splash screens *(technical)*  
-threat of demotion *(managerial)*  
-front reception desk *(operational)*  
-posted warning signs *(physical)*  

**Detective control types**  
-identify and log an intrusion attempt  
-may not prevent access  

-collect and review system logs *(technical)*  
-review login reports *(managerial)*  
-regularly patrol the property *(operational)*  
-enable motion detectors *(physical)*  

**Correction control types**  
-apply a control after an event has been detected  
-reverse the impact of an event  
-continue operating with minimal downtime  

-restoring from backups can mitigate a ransomware infection *(technical)*  
-create policies for reporting security issues *(managerial)*  
-contact law enforcement to manage criminal activity *(operational)*  
-use a fire extinguisher *(physical)*  

**Compensating control types**  
-control using other means  
-existing controls arn't sufficient  
-may be temporary  

-firewall blocks a specific application instead of patching the app*(technical)*  
-implement a separation of duties *(managerial)*  
-require simultaneous guard duties *(operational)*    

**Directive control types**  
-direct a subject towards security compliance  
-a relatively weak security control  

-store all sensitive files in a protected folder *(technical)*  
-create compliance policies and procedures *(managerial)*  
-train users on proper security policy *(operational)*  
-post a sign for "Authorized personal" *(physical)*  
  
    
---

# ***1.2 Security Concepts***  
## ***The CIA Triad***  

**Combination of principles**  
-the fundamentals of security  
-sometimes referred to as the AIC triad  

**CONFIDENTIALITY**  
-prevent disclosure of information to unqualified individuals or systems  

**INTEGRITY**  
-messages can't be modified without detection  

**AVAILABILITY**  
-Systems and networks must be up and running  

### **Confidentiality**  
-certain information should only be known to certain people  
-prevent unauthorized information disclosure  

**Encryption**  
-encode messages so only certain people can read it  

**Access Controls**  
-selectively restrict access to a resource  

**Two-factor Authentication**  
-additional confirmation before information is disclosed  

### **Integrity**  
-data is stored and transferred as intended  
-any modification to the data would be identified  

**Hashing**  
-map data of an arbitrary length to data of a fixed length  

**Digital Signature**  
-mathematical scheme to verify the integrity of data  

**Certificates**  
-combine with a digital signature to verify an individual  

**Non-repudiation**  
-provides proof of integrity, can be asserted to be genuine  

### **Availability**  
Information is accessible to authorized users   
-always at your fingertips  

**Redundancy**  
-build services that will always be available  

**Fault Tolerance**  
-systems will continue to run, even when a failure occurs  

**Patching**  
-stability  
-close security holes  

## ***Non-Repudiation***  
Adds a different perspective of cryptography  
-proof of integrity  
-proof of origin, with high assurance of authenticity  

### **Proof of Integrity**  
Verify data does not change  
-the data remains accurate and consistent  

In cryptography, we use a hash  
-represents data as a short string of text  
-a message digest, a fingerprint  

If the data changes, the hash changes  
-if the person changes you get a different fingerprint  

Doesn't necessarily associate data with an individual  
-only tells you if the data has changed  

example:  
If i downloaded a large text file ans ran a hash application i will get a hash that represents everything in that file. If I, or someone else opens that file and changes one simple character and I run a hash application again, the hash will be completely different - telling me the file has been changed.  

### **Proof of Origin**  
-prove the message was not changed  

**Integrity**  
-prove the source of the message  

**Authentication**  
-make sure the signature isn't fake  

**Non-repudiation**  
-Sign with a private key  
-the message doesn't need to be encrypted  
-nobody else can sign this (obviously)  

**Verify with the public key**  
-any change to the message will invalidate the signature  

## ***Authentication, Authorization and Accounting***  
**Authentication**  
-you are who you say you are  

**Authorization**  
-you have access to this because we know who you are  

**Accounting**  
-we see what you are doing , login time - logout time - upload, download etc.


## ***Gap Analysis***  
Where you are, compared with where you want to be  

Work towards a known baseline  
example: NIST Special Publication 800-171 rev.2 or ISO/IEC 27001  

### **Evaluate People and Processes**  
**Get a baseline of employees**  
-formal experience
-current training  
-knowledge of policies and procedures  

**Examine the current process**  
-research existing IT systems  
-evaluate existing security policies  

**Compare and contrast**  
-evaluate existing systems  


## ***Zero Trust***  
-Must authenticate for every process  

-split the network into functional planes  
-applies to physical, virtual and cloud components  

### **Data Plane**  
-process the frames, packets and network data  
-processing, forwarding, trunking, encrypting and NAT  

### **Control Plane**  
-manages the actions of the data plane  
-define polices and rules  
-determines how packets should be forwarded  
-routing tables, session tables, NAT tables  

### **Adaptive identity**  
-consider the source of the requested resource  
-multiple risk indicators  
  -relationship to the organization, physical location, type of connection, IP address, etc.  
  -make the authenticity stronger if needed

### **Threat scope reduction**  
-decrease the number of possible entry points  

**Policy-driven access control**  
-combine the adaptive identity with a preferred set of rules  

### **Security Zones**  
Security is more than a one-to-one relationship  
-broad categorizations provide a security - related foundation  

**Where are you coming from and where are you going**  
-trusted, untrusted  
-internal network, external network  
-VPN 1, VPN 5, VPN 11  
-marketing, IT, accounting, Human Resources  

**Using the zones may be enough by itself to deny access**  
-for example, untrusted to trusted zone traffic  

**Some zones are implicitly trusted**  
-for example, trusted to internet traffic  

### **Policy Enforcement Policy**  
Subjects and Systems  
-end users, apps, non-human entities  

**Policy enforcement point PEP**  
-the gatekeeper  

**Allow, monitor, and terminate connections**  
-can consist of multiple components working together  

### **Applying trust in the planes**  
**Policy decision point PDP**  
-there's a process for making a authentication decision  

**Policy engines**  
-evaluates each access decision based on policy and other information sources  
-grant, deny or remove  

**Policy administration**  
-communicates with the policy enforcement point (PEP)  
-generates access tokens or credentials  
-tells the PEP to allow or disallow access


## ***Physical Security***  
-barricades / bollards  
-access control vestibules  
-fencing  
-video surveillance  
-guards and access badges  
-lighting  
-sensors  

### **Deception and distribution**  
**honeypot**  
-attack hackers, create a virtual world  
**honeynet**  
-a combination of honeypot, servers, work stations etc.  
**honeyfile**  
-files with fake information. eg password, text  
-if someone opens a honeyfile a notification is sent  
**Honeytokens**  
-traceable data  
-fake API credentials  
-fake emails - track usage  
-can be any king of data that can be traced  

# ***1.3 Change Management***  
### **What is change management?**  
-Create a plan to implement a change, identify stakeholders, test in a branch/sandbox, develop a reversal plan if the update fails or corrupts other systems  

### **CAB change advisory board**  

**Rollback** is reverting to a working implementation before the change, in the case of webdev it would be like merging a branch to the main, finding an issue and then deploying the version prior to the merge, ie. the working version  

### **Technical change management**  
allow list vs. deny list  
-allow- only the sites on the list are accessible.  
-deny- everything is allowed except whats on the list  

# ***1.4 Cryptographic Solutions***  
### **Public Key infrastructure**  
symmetric vs. asymmetric  
What a certificate authority does  
**Symmetric**  
-same key to encrypt and decrypt  
-doesn't scale well  
-very fast  
-less overhead  

**Asymmetric**  
-two different keys but mathematically related  
-one private key one public key  
-everyone has access to the public key, can use it to encrypt data and send it ,but only the private key can decrypt the data  
-even though the keys are mathematically related, knowing one does not allow you to derive the other  
-there is no way to reverse the math to find the private key  

**Cipher text**  
-combination of the "plane text" and public key

### **Encrypting Data**  
**Database encryption**  
-transparent encryption   
    -encrypt all database information with a symmetric key  
-record level encryption  

**Transparent encryption**  
-HTTPS  
-VPN, SSL/TLS, IPsec  
 windows - bitlocker, EFS  
 Mac OS - file vault  

 **DES**  
 -data encryption standard  

 **AES**  
 -advanced encryption standard  

 **Key stretching / key strengthening**  
 -hash a password --> hash the hash --> hash the hash of the hash --> and so on  
 -makes it much harder to bruit force  

 ### **Key exchange**  
 **Diffie-Hellman concept**  
 -DHE (Diffie-hellman ephemeral)  
 1. **Private keys** each generates a private key(kept secrete)  
 2. **Public values** Using agreed-upon math parameters, large prime number and a base, each computes a corresponding public key.  
 3. **Exchange** they exchange public values over the insecure channel  
 4. **Shared secrete** each combines their own private key with the others public key. because of the math, both arrive at the same shared secrete.  
 5. **Symmetric Key** this shared secrete becomes their symmetric key, allowing secure communication without exposing private keys  
 
 **example**  
Bob and Alice want to share encrypted data without ever sending their private keys. Each generates a private key and a corresponding public value, using agreed-upon math parameters(a large prime number and a base). They exchange public values, then each combines their own private key with the other’s public value to compute the same shared secret. This shared secret becomes their symmetric key, allowing secure communication without exposing private keys.



