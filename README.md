# Splunk-Web-Intrusion-Report

## OBJECTIVE
To investigate a suspected web server compromise affecting crestwaybank.com, using Splunk log analysis to identify the attacker's initial access vector. This project involves querying the crestway-web index to reconstruct the intrusion timeline, uncover attacker behavior, and extract indicators of compromise (IOCs) from the web server logs.

## SKILLS LEARNED
- Authored a detailed 7-page incident response report documenting each investigation phase, supported by screenshots, evidence, and figure summaries.
- Extracted a comprehensive set of IOCs including IP addresses, file paths, vulnerable endpoints, plugin names, decoded commands, and attacker tools (WPScan, Netcat).
- Used Splunk’s Search Processing Language (SPL) to investigate web server logs from the crestway-web index, filtering relevant events.
- Detected brute-force login attempts via xmlrpc.php, suspicious POST requests, and reverse shell payloads by writing targeted SPL queries across access logs and HTTP request data.
- Analyzed shifts in User-Agent strings (from WPScan to Firefox) to distinguish between automated scanning and manual attacker interaction post-compromise.
- Detected a Netcat-based reverse shell encoded in a URL query string and decoded the payload using CyberChef to confirm outbound command-and-control (C2) communication.

## FULL SPLUNK INCIDENT REPORT

![2025-03-28 21_05_56-SplunkFullReport - Google Docs](https://github.com/user-attachments/assets/742ed7f0-fde9-4562-838e-6122e060de12)
![2025-03-28 21_06_11-SplunkFullReport - Google Docs](https://github.com/user-attachments/assets/d902e982-868c-43e9-8600-aea239d2ec79)
![2025-03-28 21_06_26-SplunkFullReport - Google Docs](https://github.com/user-attachments/assets/01f8e20b-b00d-4d35-99d3-3b220cd7f6f8)
![2025-03-28 21_06_41-SplunkFullReport - Google Docs](https://github.com/user-attachments/assets/967a2cb8-8963-4288-bfef-d8d323ac2ed5)
![2025-03-28 21_06_56-SplunkFullReport - Google Docs](https://github.com/user-attachments/assets/a6c65bee-4ffe-4c6f-b7b7-0d9272b5515d)
![2025-03-28 21_07_09-SplunkFullReport - Google Docs](https://github.com/user-attachments/assets/3fb94a47-0259-4b31-9809-378a2bc87b7b)
![2025-03-28 21_07_25-SplunkFullReport - Google Docs](https://github.com/user-attachments/assets/90036bff-c195-4d20-bf5d-74f7d852e32d)










