## Lab: Live Web Reconnaissance (Dirb)
Category: Offensive Security  
Target: http://testphp.vulnweb.com  
Tool: Dirb (Kali Linux Terminal)

## Lab Objective
To use a dictionary based brute force tool to discover hidden directories on a live web server and evaluate the security risk of exposed paths.

## Execution
1. Opened the "Terminal Emulator" in Kali Linux.
2. Executed the command: `dirb http://testphp.vulnweb.com`
3. Finding: Identified the `/admin` directory with an **HTTP 200 OK** status.

## Risk Analysis
The discovery of an `/admin` directory indicates a potential entry point for unauthorized users. If the administrative interface is not properly secured with multi-factor authentication (MFA), an attacker could gain control over the website's content and user data.

## Remediation
1. Rename administrative directories to something non-obvious.
2. Restrict access to the `/admin` path by IP address.
