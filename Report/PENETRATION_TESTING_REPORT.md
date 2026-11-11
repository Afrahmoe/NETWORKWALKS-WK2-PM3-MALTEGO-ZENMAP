# PENETRATION TESTING REPORT 

FOOTPRINTING & NETWORK SCANNING PHASES 

W2-PM-FINAL | CYBERSECURITY | NETWORKWALKS 

|**Pentester Name**|**Ifrah Mohamed**|
|---|---|
|**(Cybersecurity Professional)**||
|**Program/Batch**|B084-Networkwalks|
|**Date**|11 Nov 2026|
|**Modules completed**|W2-PM3 (Maltego tool)<br>W2-PM5 (Zenmap Scanning)|
|**Client/Target**|1. Networkwalks (secured written permission already)<br>2. My own local LAN Network|
|**Permission secured from client?**|Yes|
|**Phases covered**|**Phase 1:**Reconnaissance & Footprinting<br>**Phase 2:**Scanning & Network Discovery<br>**Phase 3:**Report Writing|



## 1. Liability Disclaimer

I performed these activities only on systems and devices for which I had secured written permission or that I personally own. This material is intended for educational and research purposes only. It must not be used to break the law. The instructor, the authors, and Networkwalks are not responsible for any misuse of this knowledge. Every action taken using this information is the user's own responsibility. Misuse may result in criminal charges, significant fines, loss of employment, and a permanent record. In most countries, unauthorized access is a crime, even when no damage is caused. 

## **2. Introduction** 

This report covers footprinting of the networkwalks.com domain using Maltego on Kali Linux (W2-PM3) and scanning of my own local network using Zenmap (W2-PM5). One module 

focuses on the footprinting phase, while the other focuses on the scanning phase. Together, they demonstrate how an attacker may move from gathering publicly available information to identifying live hosts on a network. This report documents the Week 2 activities of my ongoing internship program at Networkwalks. 

Both the footprinting and scanning activities were performed in Kali Linux. The evidence section documents the steps followed, the results observed, and supporting screenshots. The findings are also considered from a security perspective to explain why they may matter to an organization. 

## **3. Tools Used** 

The table below lists the tools used in this report and describes their purposes. 

|**TOOLS**|**PURPOSE**|
|---|---|
|**Kali Linux**|Operating system environment used to run the<br>footprinting and network-scanning tools.|
|**Maltego**|Used to perform domain footprinting and identify<br>publicly available information associated with<br>networkwalks.com.|
|**Zenmap (Nmap GUI)**|Used to perform a ping scan of the local LAN, identify<br>live hosts, and view the network topology.|



## **4. Activities Performed** 

## **4.1 Footprinting & Reconnaissance** 

I used Maltego on Kali Linux to conduct footprinting against the networkwalks.com domain. The objective was to identify publicly available information associated with the domain. After configuring Maltego and creating a Domain entity for networkwalks.com, I ran the available email-related transform. The transform returned info@networkwalks.com. This finding shows how publicly available contact information may be collected during the reconnaissance phase. The practical steps and screenshots are presented in Section 8.1. 

I performed reconnaissance against the networkwalks.com domain using Maltego. 

## **4.2 Network Scanning with Zenmap** 

I used Zenmap to perform a Ping Scan of my own local LAN. The scan identified two live hosts, with the IP addresses 10.0.0.1 and 10.0.0.2. I also recorded the MAC addresses displayed by the scan and reviewed the network topology in Zenmap. The topology graphic was exported as a PDF. This activity demonstrated how network discovery can help identify active devices and provide a visual overview of a network. The practical steps and screenshots are presented in Section 8.2. 

## **5. Risk Analysis & Impact** 

The exercises demonstrated how information collected during footprinting and network scanning may be useful during security reconnaissance. The following points describe potential risks associated with the observations; they are not confirmed vulnerabilities. 

### **5.1 Publicly Available Contact Information** 

The discovery of info@networkwalks.com shows that an organizational email address was returned by the email-related Maltego transform. Publicly available contact information may be misused in phishing or social-engineering attempts. The discovery alone does not demonstrate that the mailbox is vulnerable or compromised. 

### **5.2 Network Discovery Information** 

The Zenmap scan identified two live hosts on my own local LAN and displayed their IP and MAC addresses. Such information can help someone understand which devices are active on a network. If obtained by an unauthorized person, it could support further reconnaissance. The ping scan did not establish that any ports were open, that services were exposed, or that a device was vulnerable. 

### **5.3 Network Topology Visibility** 

The topology view provided a visual representation of the hosts discovered by the scan. Network diagrams can reveal useful structural information, so access to internal network maps should be limited to authorized personnel. 

## **6. Recommendations** 

Based on the observations from these exercises, the following measures may help reduce the potential risks associated with information exposure and network discovery. 

### **6.1 Email and Phishing Protection** 

Provide regular security-awareness training, encourage employees to report suspicious messages, and use appropriate email authentication and filtering controls, including SPF, DKIM, and DMARC where applicable. 

### **6.2 Network Access and Device Management** 

Maintain an inventory of authorized devices, restrict network access to approved users and devices, and use network segmentation where appropriate. Review firewall rules and investigate unfamiliar devices or unexpected changes in the network. 

### **6.3 Monitoring and Maintenance** 

Keep operating systems and network devices updated, monitor network activity for unusual behavior, and conduct regular security assessments within an approved scope. Review publicly available organizational information periodically and take appropriate steps to reduce unnecessary exposure. 

## **7. Conclusion** 

This Week 2 project provided practical experience with two important activities in penetration testing: footprinting and network scanning. Using Maltego, I performed reconnaissance against networkwalks.com and identified an associated email address returned by an email-related transform. Using Zenmap, I scanned my own local LAN, identified two live hosts, recorded their IP and MAC addresses, and reviewed the network topology. These activities helped me understand how publicly available information and network-discovery results can contribute to the reconnaissance process. They also reinforced the importance of protecting organizational information, maintaining visibility over network devices, and conducting security assessments responsibly and only with proper authorization. 

