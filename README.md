# 🛡️ Hackathon - CTF Guideline

Welcome! This guide will help you follow the key steps to participate in the cybersecurity challenges, including platform access, learning resources, and attacking vulnerable virtual machines.

---

## 📋 Main Hackathon Tasks
***Login to the WiFi Hackathon 5G / Password is Hackathon***

1. **[Bandit - Wargames](https://overthewire.org/wargames/bandit/)**
   - Learn and practice Linux command-line basics in a gamified environment.
   - Recommended levels: **Level 0 to Level 10**
   - Focus on: `ls`, `cat`, `find`, `grep`, `ssh`, `file`, `base64`, `cut`, `xxd`, `chmod`, etc.

2. **Linux Fundamentals on Google Colab**
   - Download 00_Linux_Fundamentals.ipynb from this repository and upload to Google Collab (https://colab.google/). Run and test Linux commands directly in the browser. You can also run the commands on your ParrotOS or Kali Linux machine.
   - Use this for:
     - Basic Linux commands
     - Scripting practice
     - File operations
     - Permissions and user roles

3. **Login to CTF Platform**
   - **Target IP:** `192.168.0.199`
   - Make sure you're connected to the Hackathon network (WiFi or Ethernet).
   - Open the IP address on the browser.
   - Register on the platform and explore the available CTF scenarios.

4. **CTF Challenge: Mr. Robot VM**
   - **Target:** A virtual machine modeled after the Mr. Robot TV series.
   -  The machine has the MAC Address finishing in *****555. Do the netdiscover or arp-scan -l command to find out.
   - Use tools like `nmap`, `gobuster`, `dirb`, `hydra`, and `Burp Suite`.
   - Basic flow:
     1. Reconnaissance
     2. Enumeration
     3. Exploitation (Web, SSH, Files)
     4. Privilege Escalation
     5. Capture the flag(s): typically 3 (key-1.txt, key-2.txt, root.txt)

5. **CTF Challenge: R@VEN VM**
   - Advanced exploitation and privilege escalation. The machine has the MAC Address finishing in *****DB3. Do the netdiscover or arp-scan -l command to find out.
   - Try:
     - Web attacks (XSS, SQLi, LFI/RFI)
     - CVE-based exploitation
     - Linux kernel vulnerabilities
   - Recommended tools: `nmap`, `searchsploit`, `msfconsole`, `linpeas.sh`, `pspy`, `netcat`
--- 

## 🧰 Recommended Tools

- `nmap` – Network scanning
- `netcat` / `nc` – Reverse shells
- `gobuster`, `dirb` – Directory brute forcing
- `Burp Suite` – Web app analysis
- `Hydra` – Brute-force login
- `Nikto` – Web server scanning
- `linpeas.sh`, `linenum.sh` – Privilege escalation checks
- `whoami`, `id`, `uname -a`, `sudo -l` – Local enumeration

---
