# ðŸ›¡ï¸ Cyber Security Task 02: CIA Triad & Risk Assessment

**Date:** June 14, 2026
**Intern:** Akash Yadav 
**Program:** Cybersecurity Internship

---

## ðŸ“Œ Task Objectives

- Understand the three core principles of cybersecurity: Confidentiality, Integrity, Availability
- Analyze a real-world cyber attack through the lens of the CIA Triad
- Perform a risk assessment exercise for a college environment
- Research common organizational threats and prevention methods
- Provide professional security recommendations as a security consultant

---

## âœ… Part A: Understanding the CIA Triad

### ðŸ”’ Confidentiality

**Definition:** Confidentiality ensures that information is accessible only to those authorized to view it, protecting data from unauthorized access or disclosure.

**Why it is important:** Without confidentiality, sensitive data such as financial records, medical information, and trade secrets could be exposed to unauthorized individuals, leading to privacy violations, identity theft, and loss of competitive advantage.

**Real-world example:** A hospital encrypts its patient database so that only authorized doctors and nurses can view medical records â€” administrative staff or outsiders cannot access sensitive health information.

---

### âœ”ï¸ Integrity

**Definition:** Integrity ensures that data remains accurate, complete, and unaltered except by authorized actions, throughout its entire lifecycle.

**Why it is important:** If data integrity is compromised, an organization could make decisions based on false or tampered information, leading to fraud, financial loss, or safety risks â€” especially in fields like banking or healthcare.

**Real-world example:** Software downloads include a checksum/hash value so users can verify the file hasn't been modified or corrupted (e.g., by a man-in-the-middle attacker) before installing it.

---

### âš¡ Availability

**Definition:** Availability ensures that systems, networks, and data remain accessible to authorized users whenever they are needed, with minimal downtime.

**Why it is important:** Critical services like banking systems, emergency response, and hospital systems must remain online at all times â€” downtime can result in major financial loss or even endanger lives.

**Real-world example:** A hospital's emergency patient management system stays operational 24/7, protected against DDoS attacks that attempt to flood it with traffic and take it offline.

---

### ðŸ“Š CIA Triad Comparison Table

| Principle | Definition | Why It's Important | Real-World Example |
|-----------|-----------|---------------------|---------------------|
| **Confidentiality** | Information accessible only to authorized individuals | Protects privacy, prevents data theft and identity fraud | Encrypted hospital patient database |
| **Integrity** | Data remains accurate and unaltered | Prevents fraud and bad decision-making from tampered data | Checksums to verify software downloads |
| **Availability** | Systems and data accessible when needed | Ensures critical services stay operational | Hospital systems surviving a DDoS attack |

> âœ… Visual comparison table included in `/screenshots/part_a/`

---

## âœ… Part B: Real-World Case Study â€” WannaCry Ransomware Attack

**What happened?**
In May 2017, the WannaCry ransomware attack spread rapidly across the globe, infecting over 200,000 computers in more than 150 countries within just a few days. It exploited a vulnerability in Microsoft Windows called "EternalBlue" â€” a flaw originally discovered by the NSA and later leaked publicly. Once a single machine on a network was infected, the malware self-propagated to other vulnerable machines automatically, without requiring any user interaction. It encrypted files on each infected system and displayed a ransom note demanding payment in Bitcoin to restore access. The attack severely impacted organizations including the UK's National Health Service (NHS), where hospitals had to cancel surgeries and divert ambulances because computers and medical equipment were locked.

**Which part of the CIA Triad was affected?**
Primarily **Availability** was affected, since encrypted files and locked systems meant legitimate users could no longer access their own data or critical services. **Confidentiality** was also indirectly affected, since some variants threatened to leak data if the ransom wasn't paid â€” although the main damage was operational disruption rather than data theft. Integrity was less directly impacted, since the data wasn't altered or falsified, just made inaccessible through encryption.

**What was the impact?**
The financial impact was estimated to be in the billions of dollars globally due to operational downtime, recovery costs, and lost productivity. The NHS alone reportedly lost tens of millions of pounds, with thousands of appointments and surgeries cancelled. Beyond the financial cost, the attack damaged public trust in the security of critical infrastructure and exposed how unpatched systems could create cascading global consequences.

**How could it have been prevented?**
The attack exploited a vulnerability for which Microsoft had already released a security patch nearly two months before the outbreak. The primary prevention method was simply applying that patch promptly across all systems. Additional preventive measures include network segmentation, so that a single infected machine couldn't automatically spread to the entire network, maintaining regular offline backups, so encrypted data could be restored without paying a ransom, and disabling outdated and unnecessary protocols like SMBv1, which the exploit specifically targeted.

> âœ… Case study notes included in `/screenshots/part_b/`

---

## âœ… Part C: Risk Assessment Activity

*Scenario: Acting as a Security Analyst for a college.*

| Asset | Threat | Impact | Risk Level |
|-------|--------|--------|:---:|
| Student Records | Data Breach / Unauthorized Access | Exposure of personal data, identity theft, legal liability | **High** |
| Examination Data | Tampering / Leak Before Exams | Compromised exam integrity, unfair advantage, loss of credibility | **High** |
| College Website | Defacement / DDoS Attack | Reputational damage, disrupted admissions and communication | **Medium** |
| Faculty Information | Phishing / Social Engineering | Credential theft, further network compromise, payroll fraud | **Medium** |
| Network Infrastructure | Malware / Ransomware | Complete network downtime, encrypted systems, costly recovery | **High** |
| Fee Payment System | Man-in-the-Middle / Weak Encryption | Financial fraud, stolen banking details, legal consequences | **High** |
| Campus Wi-Fi | Unauthorized Access / Rogue Devices | Network abuse, lateral movement, bandwidth theft | **Low** |

> âœ… Visual risk assessment table included in `/screenshots/part_c/`

---

## âœ… Part D: Threat Identification

### 1. Insider Threat

**Description:** An insider threat originates from someone within the organization â€” an employee, contractor, or former staff member â€” who has authorized access and either intentionally or accidentally misuses it to cause harm.

**Possible Impact:** Data theft, sabotage of systems, leaking confidential information to competitors, or accidental exposure of sensitive data through negligence.

**Prevention Methods:** Implement the principle of least privilege so employees only have access to what they need, conduct regular access audits, monitor unusual account activity, and immediately revoke access when an employee leaves the organization.

---

### 2. Malware

**Description:** Malware refers to any malicious software designed to damage, disrupt, or gain unauthorized access to a system â€” including viruses, worms, trojans, and spyware.

**Possible Impact:** Data corruption or theft, system downtime, unauthorized remote access for attackers, and potential spread to connected systems on the network.

**Prevention Methods:** Install and maintain updated antivirus/endpoint protection software, avoid downloading software from untrusted sources, and regularly scan systems for threats.

---

### 3. Phishing

**Description:** Phishing is a social engineering technique where attackers send deceptive emails or messages impersonating trusted entities to trick victims into revealing credentials or installing malware.

**Possible Impact:** Stolen login credentials leading to account takeover, financial fraud, or malware infection through malicious attachments/links.

**Prevention Methods:** Conduct regular phishing-awareness training, enable email filtering and spam detection, and verify suspicious requests through a separate official communication channel.

---

### 4. Weak Passwords

**Description:** Weak passwords are short, predictable, or reused credentials that can be easily guessed or cracked through brute-force or dictionary attacks.

**Possible Impact:** Unauthorized account access, which can be a stepping stone for attackers to access broader systems, steal data, or impersonate legitimate users.

**Prevention Methods:** Enforce strong password policies (length, complexity), implement Multi-Factor Authentication (MFA), and encourage the use of password managers.

---

### 5. Unpatched Systems

**Description:** Unpatched systems are those running outdated software with known security vulnerabilities that have not been fixed through available updates.

**Possible Impact:** Attackers can exploit known vulnerabilities to gain unauthorized access, deploy malware, or cause system-wide outages â€” as seen in the WannaCry attack (Part B).

**Prevention Methods:** Establish a regular patch management schedule, enable automatic updates where possible, and maintain an inventory of all software/systems to track what needs updating.

> âœ… Threat analysis notes included in `/screenshots/part_d/`

---

## âœ… Part E: Security Recommendations

Based on the risk assessment conducted in Part C, the following 10 security recommendations are proposed:

1. **Enable Multi-Factor Authentication (MFA)** â€” Adds a second layer of verification, so a stolen password alone cannot grant access to an account.

2. **Regular System Updates & Patch Management** â€” Closes known security vulnerabilities before attackers can exploit them, as seen with WannaCry.

3. **Strong Password Policies** â€” Reduces the risk of accounts being compromised through brute-force or credential-stuffing attacks.

4. **Employee & Staff Security Training** â€” Builds awareness so staff can recognize phishing and social engineering attempts before falling victim.

5. **Regular Automated Backups** â€” Ensures critical data (student records, exam data) can be restored quickly without paying a ransom in the event of an attack.

6. **Role-Based Access Control (RBAC)** â€” Limits access so only authorized personnel can view or modify sensitive information like grades and financial records.

7. **Network Segmentation** â€” Prevents malware from spreading freely across an entire network by isolating critical systems from general user traffic.

8. **Firewall & Intrusion Detection Systems** â€” Monitors and blocks suspicious network traffic before it reaches internal systems.

9. **Data Encryption (At Rest & In Transit)** â€” Protects sensitive data even if it is intercepted or accessed by unauthorized parties.

10. **Incident Response Plan** â€” Ensures the organization can react quickly and effectively to minimize damage when a security incident does occur, rather than reacting in a disorganized manner.

> âœ… Full recommendations doc included in `/screenshots/part_e/`

---

## âœ… Part F: Mini Security Consultant Activity

*One-page report prepared in response to: "How can we improve our cybersecurity posture?"*

### Top 5 Risks
1. Data Breach of Student Records
2. Ransomware on Network Infrastructure
3. Phishing Attacks on Faculty/Staff
4. Examination Data Tampering
5. Fee Payment System Vulnerabilities

### Top 5 Recommendations
1. Enable Multi-Factor Authentication (MFA) on all staff and admin accounts
2. Implement regular automated backups stored offline/offsite
3. Conduct mandatory security awareness training for all staff
4. Apply Role-Based Access Control (RBAC) for sensitive records
5. Keep all systems and software patched on a scheduled basis

### Expected Benefits
- Reduced risk of data breaches and unauthorized access
- Faster recovery time from ransomware or system failure
- Improved staff awareness, reducing successful phishing attempts
- Stronger compliance posture with data protection regulations
- Increased trust from students, parents, and faculty

> âœ… Full one-page formatted report included in `/screenshots/part_f/consultant_report.png`

---

## ðŸ“ Repository Structure

```
CyberSecurity_Task_02_SohamSharma/
â”‚
â”œâ”€â”€ README.md                          â† This file
â”œâ”€â”€ screenshots/
â”‚   â”œâ”€â”€ part_a/                        â† CIA Triad comparison table
â”‚   â”œâ”€â”€ part_c/                        â† Risk assessment table
â”‚   â””â”€â”€ part_f/                        â† One-page consultant report
â”œâ”€â”€ cia_triad_research.md              â† Part A detailed notes
â”œâ”€â”€ case_study_wannacry.md             â† Part B case study
â”œâ”€â”€ risk_assessment_table.md           â† Part C table
â”œâ”€â”€ threat_analysis.md                 â† Part D research
â””â”€â”€ security_recommendations.md        â† Part E recommendations
```

---

## ðŸ“ Notes

- This was a research and analytical task â€” no marks were assigned, purely for learning purposes
- Case study chosen for Part B: **WannaCry Ransomware Attack (2017)**
- All risk assessments and recommendations are hypothetical exercises for a fictional college scenario

---

## ðŸ”— Submission

Submitted via the **Sunday Submission Form** as part of Week 2 of the Cybersecurity Internship Program.

> ðŸ’¡ **Key Takeaway:** The CIA Triad â€” Confidentiality, Integrity, and Availability â€” is the foundation that every security decision is built upon. Before deploying any tool or control, a security professional must first ask: which part of the CIA Triad does this protect, and what is the actual risk to the organization?
