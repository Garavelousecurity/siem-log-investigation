# 📊 SIEM Log Investigation – Suspicious Activity Detection

## 📌 Scenario

A Security Operations Center (SOC) analyst noticed unusual activity in the SIEM dashboard.
Multiple login attempts were detected from the same IP address within a short period of time.

The purpose of this investigation is to analyze the log data and determine whether a security incident occurred.

---

## 📂 Log Data

Example SIEM log entries:

```
Timestamp            User        Source IP       Action
---------------------------------------------------------
2026-03-04 09:11:03  admin       192.168.10.25   Login Failed
2026-03-04 09:11:05  admin       192.168.10.25   Login Failed
2026-03-04 09:11:07  admin       192.168.10.25   Login Failed
2026-03-04 09:11:15  admin       192.168.10.25   Login Success
```

---

## 🔎 Investigation Findings

Indicators identified:

* Multiple failed login attempts
* Same IP address used repeatedly
* Successful login after several failures

This pattern suggests a **possible brute-force attack**.

---

## ⚠ Security Risk

Threat Type: Brute Force Attack

Potential Impact:

* Unauthorized access to privileged account
* Data exposure
* System compromise

Risk Level: High

---

## 🛠 Incident Response

Actions recommended by the SOC team:

1. Lock the affected account temporarily
2. Investigate source IP reputation
3. Reset account password
4. Enable Multi-Factor Authentication (MFA)
5. Monitor logs for further suspicious activity

---

## 🔐 Prevention Measures

Security improvements:

* Implement account lockout policy
* Monitor authentication logs continuously
* Use SIEM alerts for repeated login failures
* Enforce strong password policies

---

## 🎯 Skills Demonstrated

* SIEM log analysis
* Security incident investigation
* Threat detection
* Incident response planning
* Cybersecurity documentation
