# PowerShell Automation Basics

## Purpose

This repository contains small PowerShell scripts designed to automate common IT support and log analysis tasks.

The objective is to improve efficiency in repeatable troubleshooting workflows while reinforcing structured diagnostic processes.

All scripts are intentionally simple and readable to prioritize clarity and maintainability.

---

#### Environment

- Windows 10 / 11
- PowerShell 5.x+
- Local administrative privileges (where required)

---

#### Scripts Included

#### 1. Get-RecentFailedLogins.ps1

**Function:**  
Retrieves recent failed authentication attempts (Event ID 4625) from the Windows Security Log.

**Use Case:**  
Quickly identify repeated login failures during account lockout investigations.

**Core Logic:**
- Filters Security Log by Event ID 4625
- Sorts by timestamp
- Outputs relevant fields (TimeCreated, AccountName, LogonType)

---

#### 2. Get-NetworkConfiguration.ps1

**Function:**  
Collects and displays current network configuration details.

**Use Case:**  
Accelerate troubleshooting of connectivity and DNS-related issues.

**Core Logic:**
- Retrieves IP configuration
- Displays default gateway
- Lists DNS server entries
- Identifies active network adapters

---

#### 3. Check-ServiceStatus.ps1

**Function:**  
Checks the status of specified Windows services.

**Use Case:**  
Rapid validation of critical services during application or system troubleshooting.

**Core Logic:**
- Accepts service name as input
- Returns service status (Running, Stopped)
- Displays dependent services if applicable

---


#### Operational Benefits

- Reduces manual log filtering time
- Encourages repeatable diagnostic processes
- Minimizes human error during troubleshooting

---

#### Design Principles

- Keep scripts readable and minimal
- Avoid unnecessary abstraction
- Prioritize practical support workflows
- Ensure outputs are actionable and concise

---

#### Conclusion

This repository demonstrates foundational automation skills applied to common IT support scenarios.

The focus is not complex scripting, but operational efficiency and structured troubleshooting support — core competencies for Tier 1 support environments.
