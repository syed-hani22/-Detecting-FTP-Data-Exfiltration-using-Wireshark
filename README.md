# -Detecting-FTP-Data-Exfiltration-using-Wireshark

🛡️ Project 3: Detecting FTP Data Exfiltration using Wireshark

 📘 Description

This project demonstrates how to detect **data exfiltration** over **FTP** using Wireshark.  
We analyze a real malware-infected PCAP file where stolen password data is sent from a victim machine to an external FTP server.

---

 🕵️‍♂️ Scenario

An internal Windows machine was compromised by **Snake bro**. The malware uses the FTP protocol to **upload a stolen password file** from the victim system to a remote attacker-controlled FTP server.

This kind of activity is a classic example of **FTP-based data exfiltration**, commonly used in real-world breaches.

---

 PCAP Details

- **PCAP file used**: `2024-09-17-Snake-KeyLogger-infection-FTP-exfil.pcap`
- **Source IP (Attacker FTP Server)**: `216.252.233.118`
- **Destination IP (Victim Machine)**: `10.9.17.101`
- **FTP Username**: `chuks@lifechangerscare.com`
- **FTP Password**: `b4ST8!7!uFT9POP`

---

##  Wireshark Filters Used

```wireshark
ftp || ftp-data
