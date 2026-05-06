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
1. <img width="600" height="600" alt="Deskstop after login" src="https://github.com/user-attachments/assets/3727dab3-ba03-4d26-8dd0-7d83251d6e7f" />
- Installed Windows Server 2025 with Desktop Experience in a virtualized environment and configured initial administrative access.

2. <img width="1022" height="1037" alt="DC01 Static IP" src="https://github.com/user-attachments/assets/8843a425-ce58-49ab-833d-6e59294ae602" />
- Configured a static IP address (192.168.10.10) on the domain controller to ensure reliable network communication and proper Active Directory functionality.

3. <img width="1022" height="1035" alt="Installed ADDS" src="https://github.com/user-attachments/assets/84e9d689-9e3d-4614-9140-a65b0641c81e" />
-  Installed ADDS role on Windows Server to enable domain management and authentication services.

4. <img width="1023" height="830" alt="Showing domain login" src="https://github.com/user-attachments/assets/cd7cc59d-45b5-4ef8-baed-ccb728ba37d5" />
- Promoted the server to a Domain Controller and created the marc.local domain for centralized user authentication.

5. <img width="1080" height="1080" alt="AD Users Group OU" src="https://github.com/user-attachments/assets/92ae93ba-ea06-4fde-a4a7-15e785456ecd" />
- Created organizational units, users, and security groups to simulate a basic company structure within Active Directory.



Issues Encountered
- Initial virtual machine failed to boot into the installer because the incorrect ISO file was used. The system entered the EFI Boot Manager instead of launching Windows Setup. This was resolved by downloading the correct Windows Server ISO file and properly attaching it to the virtual machine.


Skills Demonstrated
- Windows Server installation
- Active Directory setup
- User and group management
- Domain controller configuration
- Basic DNS troubleshooting
- Technical documentation
