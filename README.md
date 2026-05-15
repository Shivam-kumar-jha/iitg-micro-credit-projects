# IIT Guwahati — Cybersecurity Micro-Credit Program

**Shivam Kumar · CBS-0249**

Hands-on project submissions from the IIT Guwahati Micro-Credit Program in Cybersecurity. Each project simulates a real-world security engagement with a defined scope, deliverables, and framework alignment.

---

## Projects

### CP1 · Security Assessment — CryptoV4ult

`cp1-iitg-submission1.pdf`

**Scenario:** Lead security engineer for a cryptocurrency platform serving 1M+ users. Tasked with a full-stack security review of a new application infrastructure.

| Section                | Coverage                                                                                                                                                   |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Secure SDLC            | Mapped 14 dev tasks to SDLC phases; added security controls at each stage (SAST, DAST, threat modeling, pen testing)                                       |
| Vulnerability Analysis | Identified brute force, session hijacking, and SQL injection in login systems; built threat matrix with impact/likelihood ratings                          |
| Container Security     | Ran Trivy scan against `vulnerables/cve-2014-6271` (Shellshock); documented 7 CVEs including CRITICAL apache2 and bash vulnerabilities with patch versions |
| API Security           | Identified BOLA, Excessive Data Exposure, and lack of rate limiting in a 3rd-party vendor API; proposed OWASP-aligned remediations                         |

**Frameworks:** MITRE ATT&CK · OWASP Top 10 · NIST CSF · CVSS v3.1

---

### CP2 · Compliance Assessment — Fed F1rst Control Systems

`cp2-iitg.pdf`

**Scenario:** Security engineer supporting a financial firm's expansion into cloud and MacBook environments. Mission: harden endpoints, write security policies, assess compliance posture.

| Section                   | Coverage                                                                                                                                       |
| ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Windows 10 Hardening      | Identified 6 misconfigurations (disabled Defender, no UAC, weak passwords, guest account active); provided remediation paths via gpedit/secpol |
| macOS Hardening           | Defined 6 pre-deployment security configurations including FileVault, Stealth Mode firewall, and SSH disablement                               |
| Security Policies         | Drafted Email Policy (5 items) and BYOD Policy security section covering iOS, Android, Windows, and macOS                                      |
| NIST SP 800-53 Compliance | Evaluated 14 controls on a Windows 10 machine; identified gaps in password policy, USB restrictions, and Defender status                       |
| CMMC Linux Compliance     | Assessed 16 CMMC controls on a Linux VM; flagged /var partition, AIDE, TCP Wrappers, and audit log configuration gaps                          |
| Cloud Build Sheet         | Produced 10-item Windows Server build standard for public cloud deployments (NSGs, IIS hardening, BitLocker, patch schedule)                   |
| CASB Analysis             | Outlined 5 key CASB benefits for cloud security: visibility, DLP, threat protection, encryption enforcement, and zero-trust access             |

**Frameworks:** NIST SP 800-53 Rev. 5 · CMMC · CIS Controls · PCI-DSS · GDPR

---

### CP3 · Securing the Perimeter — XYZ Cryptocurrency Exchange

`cp3-Submission.pdf`

**Scenario:** Contracted as a security consultant post-breach. XYZ lost 500 BTC due to a flat, unsegmented network. Tasked with redesigning their architecture and standing up a SIEM.

| Section                          | Coverage                                                                                                                                                                                          |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Network Vulnerability Assessment | Identified 3 critical issues: flat subnet with no isolation, no DMZ separation between web and DB tiers, file storage server exposed to internet                                                  |
| Network Redesign                 | Proposed segmented architecture with Public-DMZ (web servers), Private-DMZ (databases), and Internal subnet (file storage via VPN only); placed firewalls at segment boundaries                   |
| VirtualBox Lab Build             | Created DMZ VNet (Public-DMZ + Private-DMZ subnets) and Internal VNet (Internal-Subnet) in VirtualBox                                                                                             |
| SIEM Deployment                  | Deployed ELK-Server in Private-DMZ and Filebeat-VM in Public-DMZ; configured Filebeat log forwarding to Elasticsearch; verified logs in Kibana                                                    |
| Zero Trust Analysis              | Compared Continuous Monitoring, Per-Session Access, and Dynamic Access Policy against traditional models; selected Enclave Gateway as the right Zero Trust model for XYZ's segmented architecture |

**Frameworks:** Zero Trust (NIST SP 800-207) · ELK Stack · Network Segmentation · VPN

---

### CP4 · Data Security Analysis — JFin Payments

`cp4-submission.pdf`

**Scenario:** Data Security Analyst at a payment processing firm handling 100,000+ customers across the US and Europe. Responsible for governance, confidentiality, integrity, and availability of all data assets.

| Section                  | Coverage                                                                                                                                                                                                  |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Data Governance          | Evaluated 3 strategic policy items; justified annual classification and regulatory assessment cycles                                                                                                      |
| Data Classification      | Defined Confidential / Internal / Public tiers; classified 7 datasets including cardholder data, IP, and engineering diagrams                                                                             |
| Regulatory Mapping       | Mapped PCI-DSS and GDPR to Confidential data; SOX and Trade Secret laws to Internal; drafted 6 security policy items (encryption, breach notification, RBAC, retention, audit logging, vendor management) |
| Disk Encryption          | Generated RSA 2048-bit key; configured AES-XTS256-PLAIN64 disk encryption on VirtualBox VM                                                                                                                |
| File Integrity           | SHA256 hash verification on public.dll (v14.0.0.130) against baseline hash to detect tampering                                                                                                            |
| VM Security Audit        | Reviewed password policy, account lockout, audit policy, and security options via Local Security Policy; identified all-"No Auditing" gaps and zero lockout threshold                                     |
| Security Recommendations | Proposed 4 hardening steps: 14-char password minimum, 5-attempt lockout, advanced audit policy, disable RID-500 Administrator account                                                                     |
| Backup Strategy          | Recommended Daily+Weekly (7yr) for Confidential, Weekly (1yr) for Internal, Monthly (90d) for Public — aligned with SOX, GLBA, PCI-DSS                                                                    |

**Frameworks:** PCI-DSS · GDPR · SOX · GLBA · CIS Controls · ISO 27001

---

## Program Details

**Institution:** IIT Guwahati  
**Program:** Micro-Credit Program — Cybersecurity  
**Period:** Dec 2024 – Present  
**Student:** Shivam Kumar (CBS-0249) · GD Goenka University, B.Tech CSE (Cybersecurity) · CGPA 9.25
