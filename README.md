Virtual Private Network (VPN)
<p align="center">
<img src="https://i.imgur.com/MntON5Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h1>VPN - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of using a VPN.<br />

<h2>Environments and Technologies Used</h2>

- A VPN (Proton VPN)
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Steps Included</h2>

Locate Local IP
Setting Up VM Using Azure
Locating IP Through VM (France)
Connecting to VPN Through VM
Locating IP Through VPN (Japan)

<h2>Installation Steps</h2>

Find Your IP Address
Go to www.whatismyipaddress.com to see your local IP address.

<p>
<img src="https://i.imgur.com/qDgu5K6.png)" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Create an Azure Virtual Machine (VM)

Visit www.portal.azure.com.
Create a free Azure account if you don’t have one.
In the portal, go to "Virtual Machines" and create a new VM named “VM-FranceCentral,” selecting the France Central region.
  
</p>
<br />


<p>
<img src="https://i.imgur.com/K9oaS2z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


<p>
<img src="https://i.imgur.com/u3vclL3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Set Up Credentials
Choose your own username and password for the VM, and keep them secure.
  
</p>
<br />

<p>
<img src="https://i.imgur.com/rXIj3Zb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Configure Networking
Select the "Networking" tab and adjust any required settings.
  
</p>
<br />

<p>
<img src="https://i.imgur.com/OgYgNLK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Review and Create the VM

Select "Review and Create."
After validation, click "Create."
  
</p>
<br />

Find the VM’s IP Address
Once the VM is created, note its public IP address (e.g., 20.216.176.18).


<p>
<img src="https://i.imgur.com/ZlH9zI5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Log into the VM via Remote Desktop

Open Remote Desktop Connection on your local machine.
Enter the VM’s IP and the credentials you set earlier to log in.
<p>


  
</p>
<br />
<p>
<img src="https://i.imgur.com/YPBkMau.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  
</p>
<br />

<p>
<img src="https://i.imgur.com/oPJr2w2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Check the VM’s IP Address
After logging into the VM, open a browser and visit www.whatismyipaddress.com again. The IP should show as being in France
  
</p>
<br />

<p>
<img src="https://i.imgur.com/nWlX2UM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Set Up a VPN on the VM

On the local computer, create a free account on protonvpn.com.
Copy the Proton VPN URL and paste it into the VM's browser.

  
</p>
<br />

<p>
<img src="https://i.imgur.com/orO2O5y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Install and Log into Proton VPN on the VM

On the VM, download the "Windows" version of Proton VPN from the website.
Log into Proton VPN with your account credentials and connect to the VPN.
  
</p>
<br />


<p>
<img src="https://i.imgur.com/oqPHozb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Choose a Country for the VPN
In the Proton VPN app, select a country (e.g., Japan) for your VPN connection.
  
</p>
<br />

<p>
<img src="https://i.imgur.com/6Rdgg6B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Check the VPN’s IP Address
After connecting the VPN, visit www.whatismyipaddress.com on the VM again. It should show the new IP address from the VPN location (e.g., Japan).
</p>
<br />

<p>
<img src="https://i.imgur.com/lQsISWb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Summary of IP Addresses

Your home IP (USA): 137.103.51.136
VM IP (France): 20.216.176.18
VPN IP (Japan): 212.102.51.251

  
</p>
<br />
Remove the VM to Avoid Charges
If you no longer need the VM, remove it from your Azure account to avoid unnecessary charges.
