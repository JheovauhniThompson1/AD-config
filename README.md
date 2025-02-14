<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Configuring Active Directory within Azure VMs</h1>
This tutorial outlines the Setup and creation of Active directory using two Virtual machines: One for the Windows Server(Domain Controller) and a Regular Windows 10 VM.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Configuration Steps</h2>

- Created a Virtual Network and Subnet
- Created Windows Server Virtual Machine
- Created Windows 10 Virtual Machine
- Attached Windows 10 VM to Windows Server's Virtual Network and Region
- Pinged Windows Server's Private IP through windows 10 VM

<h2>Configuration Steps</h2>

<p>

<img src="https://github.com/user-attachments/assets/c252bbb7-9ff7-4a3a-80f5-d84a4a615191"/>
<img src="https://github.com/user-attachments/assets/964d52c7-0703-4233-9f6c-4b6578b6fb1a"/>

</p>
<p>
Prior to building either of the Virtual Machines, I constructed a Virtual Network called "Active-Directory_VNet". This saves me the headache of having the Virtual Machine allocated to a randomly formed Virtual Network. It also assures that both of the Virtual Machines I'll be creating can share the same Virtual Network. After completing that, I went ahead and created both Virtual Machines: a Windows Server 2022 Virtual Machine.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/76a9664d-1c40-4df3-9515-b35d6879f35f"/>
<img src="https://github.com/user-attachments/assets/3bad0287-883d-40f8-845b-d3c1bd4cc52b"/>
</p>
<p>
In this step, I retrieved the Windows Server's private IP address, then went to the Windows 10 VM's network settings -> DNS settings and entered the Windows Server's IP address as the custom DNS. Before that though I did log into the Windows Server VM and disabled its firewall as well as making its NIC private IP Address static instead of dynamic.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/1c1d3c0a-ae89-4053-9f8b-edff70d1f72a"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
