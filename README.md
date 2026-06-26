# Windows WMI Persistence Detection & Privilege Escalation Analysis

##  Project Overview
This repository contains an advanced technical analysis report and detection configurations (XML) focused on identifying, monitoring, and mitigating malicious Windows Management Instrumentation (WMI) persistence mechanisms. These methods are frequently used by threat actors for stealthy privilege escalation.

##  Business Value & Problem Solved
* **The Threat:** Attackers abuse WMI Event Subscriptions to execute malicious payloads automatically during system events or system startup, completely bypassing traditional process-monitoring controls.
* **The Solution:** Created enterprise-grade Sysmon logging filters to accurately track unauthorized WMI Event Consumers and Bindings.
* **The Outcome:** Provides incident responders and Blue Teams with a structured protocol to uncover hidden infrastructure backdoors, drastically shortening the time-to-remediate (TTR) after a breach.

##  Repository Structure
* `WMI Persistence.xml` — Advanced Sysmon monitoring filter for WMI activities.
* `Create WMI Persistence Removal & Privilege Escalation Activity Analysis.md` — Deep-dive forensic analysis, threat hunt methodology, and system remediation guide.

##  Technologies Used
* **Monitoring & Logs:** Microsoft Sysmon, Windows Event Logs (Event ID 19, 20, 21)
* **Frameworks:** MITRE ATT&CK (T1546.003 - Event Triggered Execution: WMI Event Subscription)
* **Environment:** Active Directory / Windows Enterprise Systems
