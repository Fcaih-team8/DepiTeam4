# Red Teaming Capstone Challenge – DEPIteam4

Welcome to the official repository for our Red Teaming Capstone project, completed as part of the **Digital Egypt Pioneers Initiative (DEPI)** under the **TryHackMe Red Team Capstone Challenge**.

## Objective

Simulate a real-world red team attack against a fictional financial institution (*The Reserve Bank of Trimento*), demonstrating how attackers can:

- Gain initial access
- Escalate privileges
- Move laterally between domains
- Compromise critical infrastructure (Corporate, Root, Bank)
- Exploit the SWIFT financial system

## Team Members – `DEPIteam4`

- **Shahd Tamer** – Domain Compromise & SWIFT Exploitation  
- **Youssef Magdy** – Reconnaissance & Internal Enumeration  
- **Kerolos Karam** – Introduction & Scenario Setup  
- **Habiba Mohamed** – Initial Foothold & Privilege Escalation (Tier 2)  
- **Abdelrahman Khaled** – Tier 1 Domain Lateral Movement  

## Attack Flow Summary

1. **Reconnaissance (OSINT, SMTP Brute Force)**
2. **VPN Access via leaked creds**
3. **Foothold on WRK1 using RDP**
4. **Privilege Escalation to SYSTEM via Scheduled Task**
5. **Kerberoasting & Domain Lateral Movement**
6. **Unconstrained Delegation Abuse (CORP Domain)**
7. **Golden Ticket Attack (ROOT Domain)**
8. **Credential Dumping (BANK Domain)**
9. **Access to SWIFT Application & Fraudulent Transfer**

## Flags Summary

A total of **20 flags** were captured during the engagement, representing progressive access across infrastructure layers:
- From **perimeter breach**
- To **full domain compromises**
- And final **SWIFT system exploitation**

## Recommendations

- Enforce MFA across all services
- Regularly rotate service account passwords
- Restrict delegation settings
- Monitor for suspicious Kerberos ticket activity
- Harden SWIFT and financial systems with network segmentation

## Contents

- `report/` – Full red team engagement report  
- `presentation/` – Slides used for final presentation  
- `flags_summary/` – Table of captured flags  
- `screenshots/` – Key screenshots from the operation  
- `README.md` – You're here 😉

## Final Note

This capstone taught us the value of planning, teamwork, and in-depth understanding of real-world adversarial techniques.  
We hope this repository helps others learn and grow in the red teaming field.

– DEPIteam4 🇪🇬
