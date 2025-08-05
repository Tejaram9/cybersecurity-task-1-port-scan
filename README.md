# cybersecurity-task-1-port-scan
“Task 1 of Cyber Security Internship – Performed local network reconnaissance using Nmap to identify active hosts and open ports on the LAN.”
🔍 Cyber Security Internship – Task 1: Local Network Port Scan

## 🧾 Task Objective
Perform network reconnaissance on the local network using **Nmap** to identify active hosts and open ports. This task helps understand potential vulnerabilities due to exposed network services.

---

## 🛠 Tools & Environment

- **OS**: Parrot OS (Linux)
- **Tool**: Nmap (Network Mapper)
- **Scan Type**: TCP SYN scan (`-sS`)
- **Interface**: Terminal

---

## 🌐 Network Details

- **Local IP Address**: `192.168.31.201`
- **Subnet Range Scanned**: `192.168.31.0/24`
- **Command Used**:

```bash
sudo nmap -sS 192.168.31.0/24 -oN scan-results.txt

📊 Scan Results Summary
Host Name	IP Address	Open Ports	MAC Address	Vendor
jiofiber.local.html	192.168.31.1	53 (DNS), 80 (HTTP), 443 (HTTPS), 7443, 8080, 8443	FC:B0:DE:23:36:D4	Unknown
Smart_Camera-1.lan	192.168.31.16	6668 (IRC), 8000 (HTTP-Alt)	28:18:FD:36:FD:C4	Aditya Infotech
Smart_Camera.lan	192.168.31.38	6668 (IRC), 8000 (HTTP-Alt)	28:18:FD:37:46:C3	Aditya Infotech
realme-11-Pro-5G.lan	192.168.31.73	None (All ports closed)	EE:3F:56:1C:73:B2	Unknown
—	192.168.31.102	None (All ports closed)	BA:80:C7:D9:59:92	Unknown
Tejaram.lan	192.168.31.105	All ports filtered	F0:6E:0B:DD:CB:8F	Microsoft
OPPO-A79-5G.lan	192.168.31.144	None (All ports closed)	AE:29:3E:C0:12:F8	Unknown
V2202.lan	192.168.31.162	None (All ports closed)	4E:71:D1:9F:E3:C2	Unknown
(This device)	192.168.31.201	53 (DNS)	—	—
📁 Files Included

    scan-results.txt – Raw Nmap output of scanned network

    README.md – Summary and explanation of the task

    (Optional) screenshot-terminal.png – Screenshot of terminal scan command (if added)

🧠 Key Learnings

    Identified the local IP and subnet using ip a

    Executed a TCP SYN scan with Nmap to detect live hosts

    Interpreted open ports and potential exposure on networked devices

    Recognized IoT devices (e.g., Smart Cameras) running web-accessible services

    Learned the importance of minimizing unnecessary open ports for better security

🔐 Security Insight

Open ports can expose critical services like:

    HTTP/HTTPS (80, 443, 8080, 8443): May lead to vulnerabilities if web interfaces aren't secured

    Port 6668 (IRC): Common target for malware and botnet communication

    Port 53 (DNS): Can be used in DNS tunneling attacks if misconfigured

📎 References

    Nmap Documentation

    ip command manual

    Cybersecurity Port List

✅ Task Outcome

This task builds foundational network reconnaissance skills and improves understanding of network service exposure and port-based vulnerabilities — a crucial skill for any cybersecurity analyst or ethical hacker.
