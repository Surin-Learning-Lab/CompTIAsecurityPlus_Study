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

**Proof of Origin**  
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

## **Authentication, Authorization and Accounting**  








