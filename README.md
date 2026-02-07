# SOC Lab Documentation

## Overview
This lab demonstrates basic SOC traffic analysis using Wireshark.
Captured traffic includes DNS and HTTP activity from an Ubuntu VM.


## HTTP Traffic Analysis
- **Request:** GET request to example.com using `curl`
- **Source IP:** 10.0.2.15 (Ubuntu VM)
- **Destination IP:** 185.125.190.48
- **Protocol:** HTTP/TCP
- **Response:** 200 OK, Content-Type: text/html
- **Screenshots:** <img width="663" height="272" alt="Screen Shot 2026-02-06 at 10 38 56 PM" src="https://github.com/user-attachments/assets/b5d11d18-ae73-4b05-9aa5-7e92133832ee" />
<img width="318" height="170" alt="Screen Shot 2026-02-06 at 10 33 02 PM" src="https://github.com/user-attachments/assets/c13846bf-ee84-48ae-9403-39a4db406ee3" />


- **Notes:** Traffic captured using Wireshark to show normal HTTP request and response behavior.

## DNS Traffic Analysis
- **Query:** google.com
- **Source IP:** 10.0.2.15 (Ubuntu VM)
- **Destination IP:** 10.0.2.3 (VirtualBox NAT/DNS)
- **Protocol:** DNS/UDP
- **Answer:** google.com → 142.250.190.110
- **Screenshots:** <img width="754" height="284" alt="Screen Shot 2026-02-06 at 11 04 29 PM" src="https://github.com/user-attachments/assets/6acb4184-9081-47f0-b3e7-0670472db429" />
<img width="356" height="177" alt="Screen Shot 2026-02-06 at 11 07 55 PM" src="https://github.com/user-attachments/assets/f47f6fd2-abb7-4bca-84cb-2c5b907b9db5" />

- **Notes:** Normal DNS resolution captured in the lab environment.
