# ***Section 2: Threats, Vulnerabilities, and Mitigations***  
## **2.1 Threat Actors**  
**Motivations include:**  
- data exfiltration  
- espionage  
- service disruption  
- blackmail  
- financial gain  
- philosophical / political beliefs  
- ethical  
- revenge  
- disruption / chaos  
- war  

**APT's** Advanced Persistent Threats  
**DoS** Denial of Service  

## **2.2 Threat Vectors and Attack Surfaces**  
### ***Common Threat Vectors***  
Attack vectors / threat vectors  
- method used by the attacker to gain access or infect the target  

#### 1. **Message board vectors** 
- one of the biggest threat vectors  
- everyone has at least of these messaging systems  
  

**Email**  
- malicious links in an email  
- links to a malicious site  


**SMS (short message services)**  
- attacks in a text message  


**Phishing attacks**  
- people want to click links  
- links in email, links sent via text or IM  


**Deliver Malware to the user**  
- attach it to the email  
- scan all attachments, never launch untrusted links  


**Social engineering attacks**  
- invoicing scams  
- cryptocurrency scams  


#### 2. **image based vectors**  
Easy to identify a text based threat , it is much more difficult to identify the threat in an image  
  
**Some image formats can be a threat**  
- the SVG (scalable vector graphic) format  
- image is described in XML (extensible markup language)  
  
**Significant security concerns**  
- HTML injection  
- Javascript attack code  
  
**Browsers must provide input validation**  
- avoids running malicious code  
XSS (cross site script)  

#### 3. **File based vectors**  
- Adobe PDF (portable document format)  
- Zip/RAR (zone information protocol) / (Roshal Archive) files  
- microsoft office  
  - does with macros  
  - add in files  
  - browser extensions  
    
#### 4. **Voice call vectors**  
**Vishing**  
- phishing over the phone  
  
**Spam ove IP**  
- large scale phone calls  
  
**War dialing**  
- it still happens, looking for unlisted numbers to gain access  
  
**Call tampering**  
- disruptive voice calls  
  
#### 5. **Removable device vectors**  
**Get around firewall**  
- the USB (universal serial bus) interface  
  
**malicious software on USB flash drives**  
- infect air gapped networks  
- industrial systems, high-security services  
  
**USB devices can act as a keyboards**  
- hacker on a chip  
  
**Data exfiltration**  
- terabytes of data can walk out the door  
- zero bandwidth used  
  
#### 6. **Vulnerable software vectors**  
**Client Based**  
- infected executable  
- known (or unknown) vulnerabilities  
- may require constant updates  
  
**Agentless**  
- no installed executable  
- compromised software on the server would affect all users  
- client runs a new instance each time  
  
#### 7. **Unsupported Systems vectors**  
**Patching is an important preservation tool  
- ongoing security fixes  
  
**Unsupported systems aren't patched  
- there might not even be an option  
  
**Outdated operating systems**  
- eventually even the manufacturer won't help  
  
**A single system could be an entry point**  
- keep your inventory and records current  
  
#### 8. **Unsecure network vectors**  
**The network connects everything**  
- ease of access for the attackers  
- view all (non-encrypted) data  
  
**Wireless**  
- outdated security protocols (WEP, Wired Equivalent Privacy), (WPA, WiFi Protected Access) and (WPA2, WiFi Protected Access II)  
- open or rogue wireless networks  
  
**Wired**  
-unsecure interfaces - No802.1X
- No 802.1X → The network relies on simpler methods like pre‑shared keys (PSK) (e.g., WPA2‑PSK, WPA3‑PSK).  
  
**Bluetooth**  
- reconnaissance  
- implementation vulnerabilities  
  
#### 9. **Open Service Ports**  
**Most network-based services connect over TCP (transmission control protocol) or UDP (user datagram protocol) port  
- an "open" port  
  
**Every open port is an opportunity for the attacker  
- application vulnerability or misconfiguration  
  
**Every application has their own open port**  
- more services expand the attack surface  
  
**Firewall Rules**  
- must allow traffic to an open port  
  
#### 10. **Default credentials**  
**Most devices have default usernames and passwords**  
-change yours!  
  
**The right credentials provide full control**  
- admin access  
  
**Very easy to find the defaults for your access point or router**  
- routerpasswords.com  
  
#### 11. **Supply chain vectors**  
**Tamper with the underlying infrastructure**  
- or manufacturing process  
  
**Managed service providers (MSP's)**  
- access many different customer networks from one location  
  
**Gain access to a network using a vender**  
- 2013 Target credit-card breach  
  
**Suppliers**  
- counterfeit network equipment  
- install back-doors, substandard performance and availability  
- 2020 fake cisco catalyst switches  
  
### ***Phishing***  
* **Vishing** - voice phishing  
* **Smishing** - SMS phishing  
  
### ***Impersonation***  
- voice calls  
- eliciting information  
- identity fraud  








