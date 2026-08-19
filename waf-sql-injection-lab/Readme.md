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
[screenshots: DVWA running, SQL injection attempt, WAF block page/logs, deny rule test]
