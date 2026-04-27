# Infrastructure-Project-Portfolio-WSUS-Patch-Governance-Case-Study
This project forms part of an infrastructure engineering portfolio focused on practical systems administration, governance, automation, and operational reliability using Microsoft enterprise technologies.

# WSUS Patch Governance and Compliance Case Study

Overview
This repository showcases a practical patch governance and compliance framework designed around Windows Server Update Services (WSUS) in a Microsoft Windows infrastructure.

The objective of this project is to demonstrate a structured approach to patch management that balances security, compliance, change control and operational uptime through governance processes, staged deployments and reporting automation.

This case study forms part of my infrastructure engineering portfolio focused on systems administration, governance, automation and operational reliability.


Problem Statement
Windows servers and endpoints require controlled patching to reduce security exposure while maintaining business continuity.

Common challenges addressed:

- Inconsistent patching across systems  
- Limited compliance visibility  
- Failed updates without structured remediation  
- Risk of untested patches impacting production  
- Lack of documented patch governance processes

---

Objective
Design and implement a repeatable patching process aligned to:

- Security best practice  
- Operational uptime  
- Compliance reporting  
- Change governance  
- Structured maintenance procedures

---

Environment
Infrastructure Components

- Windows Server 2019 / 2022 / 2025
- Active Directory  
- Hyper-V  
- WSUS  
- Domain-joined servers and endpoints  
- PowerShell automation

---

Patch Governance Model

Deployment Ring Strategy
Phased deployment model:

Ring 0 – Test/Pilot
- Lab systems
- IT pilot devices
- Non-production servers

Ring 1 – Standard Production
- Lower-risk production workloads
- General endpoints

Ring 2 – Critical Production
- Core infrastructure systems
- High availability workloads

---

Patching Process

Patch Lifecycle
```text
Approve → Test → Deploy → Verify → Report → Remediate
```

Process Includes
- Update approval and classification review  
- Pilot testing before production rollout  
- Scheduled maintenance window deployments  
- Post-install validation  
- Failed update remediation tracking  
- Documentation and change control

---

Compliance Reporting
PowerShell reporting examples include:

- Installed KB audits  
- Pending reboot detection  
- Last patch date reporting  
- Failed patch visibility  
- Compliance export reporting

Example use cases:
```powershell
Get-HotFix
Get-HotFix | Sort InstalledOn -Descending
```

---

Governance Controls
Implemented controls include:

- Patch testing approvals  
- Maintenance scheduling  
- Patch exception management  
- Rollback considerations  
- Remediation documentation  
- Audit readiness evidence

---

Outcomes
This approach improves:

- Patch compliance visibility  
- Vulnerability reduction  
- Operational stability  
- Structured maintenance processes  
- Repeatable governance controls

Key outcomes:
- Improved patch visibility  
- Reduced exposure to missing updates  
- Standardized remediation procedures  
- Better alignment between security and uptime

---

Repository Contents
```text
docs/       Case study documentation
scripts/    PowerShell compliance scripts
runbooks/   Operational patching procedures
diagrams/   Patch ring and process diagrams
```

---

Skills Demonstrated
- Patch Governance  
- WSUS Administration  
- PowerShell Automation  
- Windows Server Administration  
- Compliance Reporting  
- Change Management  
- Infrastructure Operations

---

Future Enhancements
Planned enhancements:

- Compliance dashboards  
- Automated reporting scripts  
- Vulnerability scan integration  
- Advanced patch SLA tracking  
- Intune / MECM co-management exploration

---

Author
Michael Francis 
Infrastructure Engineering Portfolio Project  
MGR Technologies
````

Full Case Study
Detailed PDF case study available in /docs:
- WSUS-Patch-Governance-Case-Study.pdf
