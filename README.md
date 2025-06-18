# Nmap Port Scanning
## Objectives
Use Nmap, a port scanner and network mapping tool to detect threats and vulnerabilities on a system.
## Background / Scenario
Network Mapper, or Nmap, is an open source utility used for network discovery and security auditing. Administrators also use Nmap for monitoring hosts or managing service upgrade schedules. Nmap determines what hosts are available on a network, what services are running, what operating systems are running, and what packet filters or firewalls are running.
## Required Resources
PC with Ubuntu 16.0.4 LTS installed in a VMware workstation.

### Step 1: Open a terminal window in Ubuntu.
Log in to Ubuntu:<br/>
**User:** cisco <br/>
**Password:** password <br/>

### Step 2: Run Nmap.
At the command prompt, run a basic scan against this Ubuntu system:<br/>
cisco@ubuntu:~$ nmap localhost<br/>
Open Ports: Port 22, Port 23, Port 631<br/>

### Step 3: Use administrative privileges with Nmap.
- Scan computer’s UDP ports and enter the password password when prompted: cisco@ubuntu:~$ sudo nmap –sU localhost <br/>
Open Ports: UDP 631, UPD 5353<br/>
- Version detection: cisco@ubuntu:~$ nmap –sV localhost<br/>
### Step4: Capture SSH keys.
Initiate a script scan: cisco@ubuntu:~$ nmap –A localhost

<img src="https://github.com/user-attachments/assets/a12181ff-029b-4c5b-b14e-631a3ca7efb3" width="400">
