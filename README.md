# NETWORKWALKS Cybersecurity Internship - Week 2 - Project Module 4 - Project Module 5

## A practical penetration testing assessment demonstrating OSINT reconnaissance with theHarvester and network discovery using Zenmap, with documented findings, risk analysis, and security recommendations.

### Penetration Testing Report — Reconnaissance & Network Discovery

### Overview

This project documents a practical penetration testing exercise focused on two important stages of a security assessment:
Reconnaissance using theHarvester
Network discovery and scanning using Zenmap
The purpose of this project was to understand how publicly available information can be gathered about an authorized target and how network scanning can be used to identify active hosts within an authorized local network.
All activities documented in this repository were performed in an authorized training environment for educational and cybersecurity learning purposes.


### Objectives

The main objectives of this assessment were:

&#9679; Understand the reconnaissance phase of penetration testing.

&#9679; Gather publicly available information about an authorized target.

&#9679; Identify potential information exposed through public sources.

&#9679; Determine the local IP address and LAN subnet of the testing system.

&#9679; Discover live hosts within the authorized local network.

&#9679; Identify IP addresses and MAC addresses of discovered hosts.

&#9679; Understand the security implications of information exposure and network discovery.

&#9679; Document observations, findings, risks, and recommendations.


### 🛠️ Tools Used
theHarvester - OSINT and passive reconnaissance 

Zenmap - Network discovery and Nmap-based scanning

Kali Linux - Testing environment


### 🔎 Phase 1 — Reconnaissance with theHarvester
What is theHarvester?

theHarvester is an OSINT (Open-Source Intelligence) reconnaissance tool used to collect publicly available information about a target.

It can gather information such as:

Email addresses
Subdomains
Hostnames
IP addresses
URLs
Other publicly available information
Purpose

The tool was used to understand what information about the authorized target could be discovered from publicly available sources without directly exploiting the target.

Activities Performed
Identified the authorized target domain.
Performed passive reconnaissance using theHarvester.
Collected publicly available information associated with the target.
Reviewed discovered domains, subdomains, email addresses, hostnames, and IP-related information.
Documented the reconnaissance results.
Security Relevance

Information discovered during reconnaissance can potentially help an attacker understand an organization's external attack surface.

For example, publicly exposed email addresses may be useful for phishing or social engineering, while exposed subdomains and hostnames may provide information about the organization's infrastructure.


### 🌐 Phase 2 — Network Discovery with Zenmap
What is Zenmap?

Zenmap is the graphical user interface for Nmap. It provides a convenient way to perform network discovery and security scanning.

For this practical, Zenmap was used to identify active devices within the authorized local subnet.

Activities Performed
Identified the local IPv4 address of the Windows system.
Identified the subnet mask.
Calculated the LAN subnet.
Configured Zenmap to scan the authorized local subnet.
Identified live/active hosts.
Recorded discovered IP addresses.
Recorded MAC addresses where available.
Reviewed the scan results to understand the devices present on the network.
Network Configuration

The testing system was connected to the internet using a mobile hotspot.

The local network used a private IP address in the 172.20.x.x range.

The subnet mask identified during the assessment was:

255.255.255.240

This corresponds to:

/28

The exact IP address and subnet used during the practical have been omitted from this public repository where appropriate to avoid unnecessarily exposing network information.


### 📊 Findings
Finding 1 — Publicly Available Information Exposure
Observation

theHarvester was able to identify publicly available information associated with the authorized target.

### Potential Impact

Publicly available information may assist an attacker during reconnaissance and could potentially be used for:

Phishing
Social engineering
Identifying organizational infrastructure
Identifying potential attack targets
Risk

Medium

### Recommendation

Organizations should regularly review publicly available information and remove unnecessary sensitive or technical information wherever possible.

### Finding 2 — Discoverable Network Hosts
Observation

Zenmap successfully identified live hosts within the authorized local subnet and provided information such as IP addresses and, where available, MAC addresses.

### Potential Impact

Network discovery can help an unauthorized attacker understand the devices present on a network and identify potential targets for further assessment.

Risk

Medium

### Recommendation

Organizations should implement appropriate network segmentation, firewall rules, access controls, and network monitoring to limit unauthorized network discovery and access.

### 🔐 Security Recommendations

Based on the assessment, the following recommendations are suggested:

Minimize publicly exposed information
Remove unnecessary technical information from public sources.
Protect employee email addresses
Avoid unnecessarily exposing large numbers of organizational email addresses.
Implement email security controls
Use SPF, DKIM, and DMARC to help protect against email spoofing and phishing.
Monitor publicly available information
Regularly review search engines and OSINT sources for sensitive organizational information.
Remove unnecessary subdomains
Decommission unused subdomains and avoid exposing unnecessary development or testing environments.
Secure network devices
Ensure that only authorized devices can connect to the organization's network.
Implement network segmentation
Separate sensitive systems and devices into appropriate network segments.
Use firewalls and access controls
Restrict unnecessary network traffic and services.
Perform regular security assessments
Conduct authorized vulnerability assessments and network scans periodically.
Provide security awareness training
Educate users about phishing, social engineering, and risks associated with publicly available information.



## ⚠️ Disclaimer

This project was created for educational and authorized cybersecurity training purposes.

The techniques and tools demonstrated in this repository should only be used against systems, networks, domains, and devices for which you have explicit authorization.

Unauthorized scanning, reconnaissance, or security testing may violate laws, policies, or terms of service.

👨‍💻 Skills Demonstrated
Penetration Testing Fundamentals
OSINT & Reconnaissance
Network Discovery
Nmap / Zenmap
theHarvester
IP Addressing
Subnetting
Network Security
Security Risk Identification
Security Recommendations
Technical Documentation


### 📌 Conclusion

This project provided hands-on experience with two fundamental penetration testing activities: information gathering and network discovery.

Using theHarvester, publicly available information about an authorized target was gathered and analyzed. Zenmap was then used to discover live hosts within an authorized local subnet and examine available network information.

The practical demonstrated how reconnaissance can help security professionals understand an organization's external exposure, while network discovery provides visibility into devices within a network.

Overall, this project strengthened practical knowledge of OSINT, network scanning, IP addressing, subnetting, and penetration testing methodology, while emphasizing the importance of conducting security testing only within an authorized environment.
