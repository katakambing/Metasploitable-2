# Metasploitable 2 - CTF Walkthrough

Target IP: 10.0.2.5  
Scanner used: Nmap  
Date: 30 June 2025  
Author: (aka katakambing)

---

## Note

This walkthrough documents the enumeration and exploitation of services found running on Metasploitable 2. Each step outlines the commands used, observations made, and outcomes of exploitation attempts. This is for educational and portfolio-building purposes only. Do not attempt unauthorized access on systems you do not own or have explicit permission to test.

---

## 1. Initial Port Scan

Command:
bash
nmap -sS -p- 10.0.2.5

Output summary:
Host is up with 33 open TCP ports.
Services running include: FTP, SSH, Telnet, SMTP, SMB, MySQL, PostgreSQL, VNC, AJP, and more.

Open Ports:
21/tcp     - FTP
22/tcp     - SSH
23/tcp     - Telnet
25/tcp     - SMTP
53/tcp     - DNS
111/tcp    - rpcbind
139/tcp    - NetBIOS-SSN
445/tcp    - Microsoft-DS
512-514    - r-services
1099/tcp   - RMI Registry
2049/tcp   - NFS
2121/tcp   - ccproxy FTP
3306/tcp   - MySQL
3632/tcp   - DistCC
5432/tcp   - PostgreSQL
5900/tcp   - VNC
8009/tcp   - AJP13
8180/tcp   - Unknown HTTP
8787/tcp   - msgsrvr
45156+     - Unknown high ports


