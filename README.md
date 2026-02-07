# SOC Lab Documentation

## Overview
This lab demonstrates basic SOC traffic analysis using Wireshark.
Captured traffic includes DNS and HTTP activity from an Ubuntu VM.

## Folder Structure
- `Evidence/` → Screenshots of captured traffic
- `Captures/` → Wireshark `.pcap` files
- `README.md` → Documentation

## HTTP Traffic Analysis
- **Request:** GET request to example.com using `curl`
- **Source IP:** 10.0.2.15 (Ubuntu VM)
- **Destination IP:** 185.125.190.48
- **Protocol:** HTTP/TCP
- **Response:** 200 OK, Content-Type: text/html
- **Screenshots:** `Evidence/HTTP_Request.png`, `Evidence/HTTP_Response.png`
- **Notes:** Traffic captured using Wireshark to show normal HTTP request and response behavior.

## DNS Traffic Analysis
- **Query:** google.com
- **Source IP:** 10.0.2.15 (Ubuntu VM)
- **Destination IP:** 10.0.2.3 (VirtualBox NAT/DNS)
- **Protocol:** DNS/UDP
- **Answer:** google.com → 142.250.190.110
- **Screenshots:** `Evidence/DNS_Request.png`, `Evidence/DNS_Response.png`
- **Notes:** Normal DNS resolution captured in the lab environment.
