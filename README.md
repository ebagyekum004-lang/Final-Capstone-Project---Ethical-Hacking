# Final-Capstone-Project---Ethical-Hacking

# Final Capstone Project Report

**Ethical Hacking & Penetration Testing Assessment**

---

## Executive Summary

This report documents a controlled penetration testing engagement conducted against a simulated enterprise environment to identify, exploit, and assess common security vulnerabilities. The objective was to evaluate system resilience against real-world attack techniques and provide actionable remediation recommendations. The assessment covered web applications, web server configurations, SMB file-sharing services, and network traffic analysis. Multiple vulnerabilities were successfully identified and exploited, demonstrating risks related to improper input validation, insecure service configuration, weak access controls, and unencrypted data transmission.

---

## Scope Definition

### In Scope

* Web application hosted on **10.5.5.12**
* SMB servers within the **10.5.5.0/24** network
* Network traffic captured in **SA.pcap**
* Authorized use of exploitation and enumeration tools
* Credential testing and file access within the lab environment

### Out of Scope

* Denial-of-Service (DoS) attacks
* Privilege escalation beyond defined challenge objectives
* Attacks against systems outside the provided IP ranges
* Persistent malware deployment or system modification
* Any testing on production or unauthorized systems

---

## Penetration Testing Methodology

The assessment followed a structured penetration testing lifecycle aligned with industry standards such as **PTES** and **NIST SP 800-115**:

1. Planning and Authorization
2. Reconnaissance and Enumeration
3. Vulnerability Identification
4. Exploitation
5. Post-Exploitation Analysis
6. Remediation and Risk Evaluation

---

## Reconnaissance & Enumeration

Initial reconnaissance involved identifying active hosts, services, and exposed resources. Tools such as **Nmap**, **Nikto**, **Enum4Linux**, **SMB client utilities**, and **Wireshark** were used to enumerate open ports, running services, directory structures, SMB shares, and unencrypted network traffic. This phase revealed misconfigured services, accessible directories, and insecure communication channels.

---

## Key Activities Performed

* Exploited **SQL injection** vulnerabilities to extract database credentials and gain unauthorized system access
* Identified **web server misconfigurations** allowing directory listing and unauthorized file discovery
* Enumerated and accessed **unsecured SMB shares** without valid authentication
* Analyzed **PCAP traffic** to recover sensitive information transmitted in clear text
* Retrieved challenge flags by chaining reconnaissance findings with exploitation techniques
* Assessed security posture and documented weaknesses with supporting evidence

---

## Outcomes and Findings

The engagement successfully demonstrated how common security weaknesses can be exploited to compromise confidentiality and access sensitive data. Key outcomes included:

* Successful credential extraction via SQL injection
* Discovery of sensitive configuration files through directory indexing
* Unauthorized access to SMB shares and file upload capability
* Exposure of usernames, passwords, and files through unencrypted traffic analysis

Each vulnerability highlighted potential real-world risks such as data breaches, lateral movement, and credential compromise.

---

## Testing Environment

All testing was conducted in a **controlled laboratory environment** provided as part of the Ethical Hacking Capstone Project. No production systems were targeted, and all activities complied with ethical hacking principles and authorization guidelines.

---

## Conclusion

This penetration testing assessment demonstrates practical, hands-on experience with real-world attack vectors and defensive considerations. The project reflects a strong understanding of attacker methodologies while maintaining a focus on risk mitigation and security improvement. The techniques and remediation strategies applied align with modern enterprise security expectations and industry best practices.

---

## Recommended Next Steps

* Implement secure coding practices and parameterized queries
* Harden web server configurations and disable directory listing
* Enforce strong authentication and restrict SMB access
* Encrypt data in transit using TLS, VPNs, or IPsec
* Conduct regular security assessments and monitoring

---

**End of Report**
