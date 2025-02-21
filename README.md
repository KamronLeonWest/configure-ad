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
</p>
<p>
First, create a resouce group. Name this what ever you like.
</p>
<p>
<img src="https://imgur.com/aQleFIa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, you're going to need to make two virtual machines: one with the image Windows Server 2022 and the other will be Windows 10
</p>
<p>
<img src="https://imgur.com/BcQ079S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From here, you will have automatically created the subnet by default. Do not change these settings
</p>
<p>
<img src="https://imgur.com/KH1A5iS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In order to log into the virtual machines, you will need to create a basic username and password. These credentials will be essential when configuring administrative users
</p>
<p>
<img src="https://imgur.com/Rj6qMyj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After creating the virtual machines, navigate to the Windows Server 2022 (named dc-1 for me) VM's settings to change the IP settings
</p>
<p>
<img src="https://imgur.com/rvh6Tqk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The Windows Server 2022 VM, or dc-1 VM (domain controller virtual machine), will need to be set to static so the other VM can connect to it
</p>
<p>
<img src="https://imgur.com/DPvV7rx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once the dc-1's settings are configured, go to the Windows 10 VM settings (client-1 for me)
</p>
<p>
<img src="https://imgur.com/78e0jnc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On the DNS servers tab, change the value to the same IP address as the static IP of the dc-1 VM
</p>
<br />

<p>
<img src="https://imgur.com/sDaj3tY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Log into the dc-1 VM, click the start menu, then open Server Manager
</p>
<p>
<img src="https://imgur.com/oCV6cXS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On the page that opens, click 'Add roles and features'
</p>
<p>
<img src="https://imgur.com/SSQmG9K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://imgur.com/vlnwhRN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://imgur.com/D4uEHkF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://imgur.com/0kBerQg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://imgur.com/KI8v1l9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://imgur.com/yyLXJdH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/I1nsB1A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://imgur.com/dge8kut.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://imgur.com/VZLdxMa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://imgur.com/qF7fnDZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://imgur.com/k7iBjrW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://imgur.com/ATVxDix.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://imgur.com/ykofkWZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<p>
<img src="https://imgur.com/jJnSBMB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
