# Elevate Labs Cybersecurity Internship - Task 4

## Task: Setup and Use a Firewall on Windows

### Objective
Configure and test basic firewall rules to allow or block traffic using Windows Defender Firewall.

### Tools Used
- Windows Defender Firewall with Advanced Security
- Windows PowerShell
- Test-NetConnection

## Steps Performed

### 1. Checked Existing Firewall Rules
Reviewed the existing Inbound Rules and Outbound Rules in Windows Defender Firewall with Advanced Security.

### 2. Created an Inbound Firewall Rule
Created a new inbound firewall rule with the following configuration:

- Rule Name: Block Telnet Port 23 - Task 4 - Anusha
- Rule Type: Port
- Protocol: TCP
- Local Port: 23
- Action: Block the connection
- Profiles: Domain, Private, Public

### 3. Tested the Firewall Rule
Used Windows PowerShell to test connectivity to TCP port 23 on the local machine.

Command used:

```powershell
Test-NetConnection localhost -Port 23
