# cybersecurity-task1
Port scanning using Nmap for local network exposure
#Cyber Security Internship - Task 1: Local Network Port Scan

## Objective
Perform a network reconnaissance scan to identify open ports and analyze potential exposure in the local network.

## Tools Used
- Nmap (for scanning)
- xsltproc (for HTML report conversion)

## Command Executed

nmap -sS -oX res.xml 192.168.47.128/24
xsltproc res.xml -o test.html

--- Devices Found (5 Hosts Online)
192.168.47.1
192.168.47.2
192.168.47.128
192.168.47.129
192.168.47.254

🔓 Open Ports Summary
IP Address	Open Ports
192.168.47.1	- 135, 139, 445
192.168.47.2	- 53
192.168.47.128 - 21
192.168.47.129	- 21, 22, 23, 25, 53, 80, 111, 139, 445, 512, 513, 514, 1099, 1524, 2049, 2121, 3306, 5432, 5900, 6000, 6667, 8009, 8180
192.168.47.254	- No open ports detected

⚠️ Potential Security Risks
Use of insecure protocols (Telnet, FTP)
Unsecured database services exposed
Remote access ports open (VNC, X11)
Legacy services still active (NetBIOS, RPC, shell)
