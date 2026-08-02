# Wazuh SIEM Home Lab

## Overview
Deployed a Wazuh SIEM environment with a manager on Ubuntu Server (VirtualBox) 
and an agent on a Windows host, connected over bridged networking.

## What I Did
- Installed Wazuh Manager on Ubuntu Server in VirtualBox
- Installed Wazuh Agent on my Windows host machine
- Registered the agent with the manager using key-based authentication
- Configured real-time File Integrity Monitoring (FIM) on a test folder using Syscheck
- Verified the setup by creating/modifying files in the monitored folder and 
  confirming alerts appeared on the Wazuh dashboard

## Why This Matters
File Integrity Monitoring is used in real SOC environments to detect unauthorized 
changes to critical files — for example, ransomware modifying files, or an attacker 
tampering with system configurations. This lab gave me hands-on experience with the 
exact type of monitoring a SOC analyst would rely on daily.

## Screenshots
Proof the Wazuh Manager is installed and running
<img width="1597" height="898" alt="image" src="https://github.com/user-attachments/assets/b7da31ee-28cd-4426-b4d9-fe8317bab613" />

Proof you can access the Wazuh Dashboard
<img width="1601" height="901" alt="image" src="https://github.com/user-attachments/assets/e6f4ed29-d1d1-4805-b866-318dc5e47b1a" />

Proof the Windows agent is connected ("Active")
<img width="1603" height="895" alt="image" src="https://github.com/user-attachments/assets/2ef3f147-ea83-4d2d-b032-00c02251245b" />

Proof File Integrity Monitoring is working
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/cb49d7c0-1160-4256-b695-fe0c5c4f5f0e" />

The config file itself
<img width="1917" height="1077" alt="image" src="https://github.com/user-attachments/assets/8719285b-89f7-4336-93de-cd1c9f6156aa" />

