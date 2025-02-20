<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create a Resource Group, Virtual Machine, and Subnet on Azure
- Create Domain Controller Virtual Machine on Windows Server 2022, and Client Virtual Machine on Windows 10
- Set Client's DNS Settings to Domain Controller's Private IP address
- Install Active Directory Domain Services on the Domain Controller Virtual Machine
- Create Organizational Units
- Join Client Virtual Machine to the Domain
- Setup Remote Desktop for non-administrative users on Client Virtual Machine

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://imgur.com/hqctIk6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/aQleFIa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/BcQ079S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/KH1A5iS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/Rj6qMyj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/rvh6Tqk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/DPvV7rx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/78e0jnc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create two virtual machines on Azure: one for Windows Server 2022 and one for Windows 10
</p>
<br />

<p>
<img src="https://imgur.com/sDaj3tY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/oCV6cXS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/SSQmG9K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/vlnwhRN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/D4uEHkF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/0kBerQg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/KI8v1l9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/yyLXJdH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/I1nsB1A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/dge8kut.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/VZLdxMa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/qF7fnDZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/k7iBjrW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/ATVxDix.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/ykofkWZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/jJnSBMB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
