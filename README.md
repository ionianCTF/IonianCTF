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

4. **CTF Challenge: Network Forensics**
    - Tools Required: `tshark`, `Wireshark`, `NetworkMiner` (you can also use https://apackets.com/ or whatever to find deeper details using other tools). 
    - Look at the CTF challenge with the  Name Network forensics and answer the questions/flags. 
    - File: [`WebInvestigation.pcap`](#) *(Download it from the repository)*  
    - Environment: Jupyter Notebook / Google Colab compatible

6. **CTF Challenge: Mr. Robot VM**
   - **Target:** A virtual machine modeled after the Mr. Robot TV series.
   - Walkthrough: https://medium.com/@cspanias/thms-mr-robot-ctf-walkthrough-2023-55ca5c19fbaf
   - You can download the .ova if you want, but the flags are different. https://www.vulnhub.com/entry/mr-robot-1,151/
   -  The machine has the MAC Address finishing in *****555. Do the netdiscover or arp-scan -l command to find out.
   - Use tools like `nmap`, `gobuster`, `dirb`, `hydra`, and `Burp Suite`.
   - Basic flow:
     1. Reconnaissance
     2. Enumeration
     3. Exploitation (Web, SSH, Files)
     4. Privilege Escalation
     5. Capture the flag(s): typically 3 (key-1.txt, key-2.txt, root.txt)

7. **CTF Challenge: R@VEN VM**
   - Advanced exploitation and privilege escalation. The machine has the MAC Address finishing in *****DB3. Do the netdiscover or arp-scan -l command to find out.
   - Walkthrough: https://dorian5.medium.com/vulnhub-raven-1-4c7122d5569f
   - You can download the .ova if you want, but the flags are different. https://www.vulnhub.com/entry/raven-1,256/
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
