# Task 1 - Network Port Scanning

## Objective
The objective of this task is to scan the local network to discover open ports and understand network exposure and security risks.

## Tools Used
- Nmap  
- Wireshark  
- Kali Linux  

## Network Information
- IP Address: 192.168.24.128  
- Network Range: 192.168.24.0/24  

## Scan Command Used
nmap -sS 192.168.24.0/24

## Results
The scan showed that most ports were filtered and some ports like 1079, 1057, and 1718 were closed. No open ports were found.

## Analysis (Services)
Common ports like 22 (SSH), 80 (HTTP), and 443 (HTTPS) are used for remote access and web services. However, in this scan, no ports were open, indicating no active services.

## Security Risks
Open ports can expose services to attackers. Since no open ports were found, the system has a lower attack surface. Filtered ports indicate firewall protection.

## Wireshark Analysis
Wireshark captured TCP SYN packets and RST-ACK responses, indicating that connection requests were rejected and ports are closed.

## Conclusion
The system appears secure as no open ports were found and most ports were filtered or closed.
