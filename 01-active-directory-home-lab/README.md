Active Directory Home Lab: User and Computer Management

Overview
- This project demonstrates how I built a basic Windows domain environment using virtual machines. The goal was to practice Active Directory setup, user management, domain joining, and basic IT administration tasks.

Tools
- VMWare Workstation
- Windows Server 2025
- Windows 11
- ADDS

Lab Setup
- Domain Controller: DC01
- Client Computer: CLIENT01
- Domain Name: marc.local
- Network: 192.168.10.0/24

Tasks to be Completed
- Install Windows Server
- Configure static IP address
- Install Active Directory Domain Services
- Create a new domain (marc.local)
- Create users and security groups
- Install Windows 11 client VM
- Join client computer to domain
- Test domain user login

Screenshots
(to be added)

Issues Encountered
- Initial virtual machine failed to boot into the installer because the incorrect ISO file was used. The system entered the EFI Boot Manager instead of launching Windows Setup. This was resolved by downloading the correct Windows Server ISO file and properly attaching it to the virtual machine.


Skills Demonstrated
- Windows Server installation
- Active Directory setup
- User and group management
- Domain controller configuration
- Basic DNS troubleshooting
- Technical documentation
