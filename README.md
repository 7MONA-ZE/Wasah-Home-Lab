<h1>Wazuh Home Lab</h1>


<h2>Description</h2>
Wazuh SIEM/XDR Deployment & FIM Demonstration
Objective: Set up an end-to-end open-source Security Information and Event Management (SIEM) and Extended Detection and Response (XDR) lab using Oracle VM VirtualBox, deploy the Wazuh infrastructure, and demonstrate File Integrity Monitoring (FIM).


<br />


<h2>Utilities Used</h2>

- <b>WAZUH Agent</b>
- <b>WAZUH Manager</b>


<h2>Environments Used </h2>
- <b>Virtual Box</b> 
- <b>Kali Linux</b>
- <b>Windows 10 pro</b>


<h2>walk-through:</h2>
1. Lab Architecture & Environment Setup
Hypervisor: Oracle VM VirtualBox

Wazuh Manager / Server: Deployed on Linux (e.g., Kali Linux or Ubuntu/Debian VM) acting as the centralized engine for log processing, threat intelligence correlation, and alert generation.

Monitored Endpoint: Windows 10 Pro running the lightweight Wazuh Agent to collect endpoint telemetry and transmit events to the manager.

Networking: VirtualBox Internal Network or Host-Only Adapter to ensure secure communication between the Wazuh Manager and Windows endpoint.

2. Installation & Agent Deployment
Wazuh Manager Installation: Installed and initialized the Wazuh server components (Wazuh Indexer, Server, and Dashboard) on the Linux Virtual Machine.

Wazuh Agent Deployment: Installed the Windows agent on the Windows 10 Pro VM and pointed it to the Wazuh Manager’s IP address.

Agent Registration: Verified that the agent successfully established an encrypted channel with the manager and appeared as Active on the Wazuh dashboard.
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
