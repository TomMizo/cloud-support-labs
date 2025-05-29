# Azure Lab: Deploying a Windows Virtual Machine

## Overview
This lab was part of my ongoing effort to gain more hands-on experience with Azure. I created a basic Windows Server virtual machine using the Azure portal, configured remote desktop access, and successfully connected to it from my local machine.

## Objectives
- Set up a virtual machine in Azure (Windows Server 2022)
- Enable RDP access and connect remotely
- Get familiar with VM settings and the Azure deployment process

## Tools & Services Used
- Azure Portal
- Windows Server 2022
- Remote Desktop (RDP)

## Steps I Took

1. Logged into the Azure Portal and went to **Virtual Machines > Create**
2. Chose the following settings:
   - **Image:** Windows Server 2022 Datacenter
   - **Size:** B1s
   - Created username/password for login
   - Enabled **RDP (port 3389)** under networking
3. Clicked **Review + Create**, then deployed the VM
4. Once deployed, I copied the public IP
5. Opened Remote Desktop Connection on my machine and connected to the VM
6. Logged in and explored Server Manager and settings

## Outcome
I was able to deploy and connect to the virtual machine without issues. This helped reinforce how VM provisioning works in Azure and how important it is to configure networking settings correctly during setup.

## What I Learned
- Azure VM deployment is pretty straightforward once you understand the steps
- RDP access must be configured during deployment or added later via NSG rules
- Cost control matters — always shut down VMs when not in use to save credits

## Resources
- [Microsoft Learn: Create a Windows VM in Azure](https://learn.microsoft.com/en-us/azure/virtual-machines/windows/quick-create-portal)
