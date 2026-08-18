## Initial State

 Port 21 was listening: the service was managed by xinetd 

<img width="863" height="463" alt="Screenshot 2026-08-15 161033" src="https://github.com/user-attachments/assets/80dc0902-88e0-4820-9068-bafaafdc5224" />

# FTP Service Remediation
FTD service was disabled through the appropriate xinetd configuration. 

<img width="882" height="490" alt="Screenshot 2026-08-15 162123" src="https://github.com/user-attachments/assets/18dc3634-5af8-4d45-8c5d-980dca38714a" />


Verification : An Nmap scan was performed after remediation 

Result :  FTD service was no longer accepting connections on TCP Port 21. this reduces the attack surface of the metaspolitable2 system.


<img width="959" height="553" alt="Screenshot 2026-08-15 163204" src="https://github.com/user-attachments/assets/6260c936-ec0f-41c8-b180-d4f54d2d4413" />
