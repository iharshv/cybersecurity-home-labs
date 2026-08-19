# Web Application Firewall Lab — SafeLine WAF vs SQL Injection

## Overview
Built a complete attack-and-defense home lab: a vulnerable web application (DVWA) 
protected by SafeLine WAF, tested against real SQL injection attacks from Kali Linux.

## What I Did
- Set up a LAMP stack (Apache, MySQL, PHP) on Ubuntu Server and deployed DVWA 
  (Damn Vulnerable Web App) as the target application
- Configured local DNS resolution and a self-signed SSL certificate for HTTPS
- Deployed SafeLine WAF as a reverse proxy in front of DVWA
- Launched a SQL injection attack from Kali Linux against DVWA's login form
- Verified SafeLine WAF detected and blocked the injection attempt, confirmed via WAF logs
- Configured advanced WAF protections: HTTP flood/DoS defense, authentication 
  gateway sign-in, and custom IP-based deny rules (blocking the Kali attacker IP directly)

## Why This Matters
This lab demonstrates both sides of application security — exploiting a real 
vulnerability class (SQL injection, still one of the most common web attack vectors) 
and then seeing exactly how a WAF detects and stops it in real time. Understanding 
this attack-defense pair is core to both VAPT work and SOC-side monitoring.

## Evidence

### DVWA running
<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/80574b20-e878-479a-98b9-f1e5709c1f92" />

### SQL injection attempt
<img width="1919" height="1014" alt="image" src="https://github.com/user-attachments/assets/56e87594-42ec-4056-8936-d55c09b28286" />

### WAF block page/logs
<img width="817" height="649" alt="image" src="https://github.com/user-attachments/assets/07964fb8-2135-4a78-a599-8d290bea1db3" />

<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/77e2c53b-d32f-4d0c-9d0d-2e39bc13789f" />

### Deny rule test
<img width="1916" height="1019" alt="image" src="https://github.com/user-attachments/assets/2939709e-7098-4ecb-b970-25f621ee4481" />

<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/187bad7d-b5a9-414a-a1ec-9af77749717b" />
