# Threat Hunting & Incident Investigation Lab

## 📌 Project Overview
This project demonstrates proactive threat hunting and incident investigation within a Windows Active Directory environment. Instead of relying on alerts, suspicious activity was identified through manual log analysis.

---

## 🎯 Objective
- Identify malicious activity without SIEM alerts
- Analyze Windows Security logs and Sysmon data
- Investigate attacker behavior across systems

---

## 🛠️ Environment
- Domain Controller: DC01 (corp.local)
- Windows Server 2019
- Sysmon installed
- Event Viewer for log analysis

---

## 🔍 Threat Hunting Activities

### 1. Failed Login Analysis
- Event ID: 4625
- Identified repeated failed login attempts
- Detected potential brute force attack

---

### 2. Successful Login Correlation
- Event ID: 4624
- Logon Type: 3
- Identified successful login after multiple failures

---

### 3. Process Investigation
- Sysmon Event ID: 1
- Observed execution of:
  - cmd.exe
  - whoami.exe
  - ipconfig.exe

---

### 4. Network Activity Analysis
- Sysmon Event ID: 3
- Detected internal network probing activity

---

## 🧠 Key Findings
- Evidence of credential-based attack
- Post-compromise reconnaissance observed
- Indicators of lateral movement behavior

---

## 📊 Skills Demonstrated
- Threat Hunting
- Log Analysis (Windows + Sysmon)
- Incident Investigation
- Security Analysis
- MITRE ATT&CK understanding

---

## ✅ Conclusion
This lab demonstrates the ability to proactively identify and investigate security incidents without relying on automated alerts, simulating real-world SOC analyst responsibilities
