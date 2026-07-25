# Metaploitable2-home-lab-
Objective : Exploit a vulnerable service in metasploitable 2 

Lab setup: VM kali and metasploitable2 

Commands execuated: 

| ipconfig or ipaddr |            | ping Nmap -sV  (ipaddr)|           | namp -sV -p21  | 

Nmap -sV  (ipaddr)        

namp -sV -p21
----------------------------------------------------------------------------------------------------------
msfconsole (to start metaploit) 

use    

info            

show options

set (set the necessary parameters RHOST refers to the target's IP , LHOST refers to the attacker's) 

run 

<img width="956" height="494" alt="Screenshot 2026-07-24 151708" src="https://github.com/user-attachments/assets/4bef9547-df4e-4c65-a5e1-ce6c8b189b05" />

Exploit Outcome: The Metasploit module successfully exploited the vulnerable FTP service (vsftpd 2.3.4) on the Metasploitable target.A Meterpreter session was established from the attack machine , demonstrating successful remote code execution on the target system.
