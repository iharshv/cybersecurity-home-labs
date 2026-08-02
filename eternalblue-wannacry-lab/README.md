# System Hacking — EternalBlue (MS17-010) / WannaCry Simulation

## Overview
Simulated exploitation of the EternalBlue (MS17-010) SMB vulnerability — the same 
vulnerability exploited by the WannaCry ransomware in 2017 — against an isolated 
Windows 7 VM, using Kali Linux, Nmap, and Metasploit.

## What I Did
- Scanned the Windows 7 target using Nmap to identify open SMB port 445 and 
  confirm the vulnerable SMB version
- Located the appropriate exploit module in Metasploit for MS17-010
- Configured and executed the exploit against the target
- Gained a shell/session on the Windows 7 VM, confirming successful exploitation
- [Any post-exploitation steps you did]

## Why This Matters
EternalBlue/MS17-010 was the vulnerability behind WannaCry, one of the most 
destructive ransomware outbreaks in history, causing billions in damages globally. 
Understanding this exploit demonstrates knowledge of SMB protocol vulnerabilities, 
lateral movement techniques, and why patch management is critical in enterprise 
security — a lesson equally relevant to SOC defense and VAPT offense.

## Evidence
<img width="1492" height="935" alt="image" src="https://github.com/user-attachments/assets/6514e65a-f246-448e-83df-eaebb43a2754" />
<img width="955" height="732" alt="Screenshot 2026-08-03 030723" src="https://github.com/user-attachments/assets/e535b6da-e707-4abf-aec6-dd357855bb99" />
<img width="1296" height="907" alt="Screenshot 2026-08-03 030806" src="https://github.com/user-attachments/assets/9261ced7-64b9-4158-9f40-10b4c0388bf5" />
<img width="1196" height="862" alt="Screenshot 2026-08-03 030825" src="https://github.com/user-attachments/assets/efc8134a-478a-455b-bc3d-20f7ea32200e" />
<img width="1401" height="828" alt="image" src="https://github.com/user-attachments/assets/88b42ea7-ceef-4a4a-9535-04cfa2f75bdd" />
<img width="1322" height="857" alt="Screenshot 2026-08-03 030854" src="https://github.com/user-attachments/assets/9b8f30ab-1483-4f02-8561-c9cccd9ea78e" />
<img width="1917" height="955" alt="image" src="https://github.com/user-attachments/assets/94dffe3a-3e80-4944-b735-0c320fcba066" />




