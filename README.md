# nmap
# Basic Network Scan Using Nmap

## Objective
Perform a basic Nmap scan on a local virtual machine to identify open ports, running services, and system information.

## Tools Used
- Nmap 7.95
- Kali Linux Virtual Machine

## Scan Command

### Flags Explanation:
- **-sC** → Runs default Nmap scripts (NSE)
- **-sV** → Detects service versions

---

## Scan Findings

### ✔ Host Status
- Host is up and responding
- 999 TCP ports are closed

### ✔ Open Port Found
| Port | State | Service | Description |
|------|--------|----------|------------------------------|
| **22/tcp** | open | ssh | Secure Shell service running on OpenSSH 10.2p1 |

---

## Significance of Open Port 22
- Port **22** is used for SSH (Secure Shell)
- Enables secure remote access to the machine
- If exposed improperly, attackers may attempt:
  - Brute-force password attacks
  - Exploiting outdated SSH versions
  - Unauthorized access attempts

---

## Conclusion
The VM is running a single open port (22 - SSH).  
All other ports are closed, indicating a secure default configuration.  
SSH should be protected with:
- Strong passwords
- Key-based authentication
- Firewall restrictions
