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
1. <img width="1918" height="1142" alt="Deskstop after login" src="https://github.com/user-attachments/assets/3727dab3-ba03-4d26-8dd0-7d83251d6e7f" />
- Installed Windows Server 2025 with Desktop Experience in a virtualized environment and configured initial administrative access.

2. <img width="1022" height="1037" alt="DC01 Static IP" src="https://github.com/user-attachments/assets/8843a425-ce58-49ab-833d-6e59294ae602" />
- Configured a static IP address (192.168.10.10) on the domain controller to ensure reliable network communication and proper Active Directory functionality.

3. <img width="1022" height="1035" alt="Installed ADDS" src="https://github.com/user-attachments/assets/84e9d689-9e3d-4614-9140-a65b0641c81e" />
-  Installed ADDS role on Windows Server to enable domain management and authentication services.

4. <img width="1023" height="830" alt="Showing domain login" src="https://github.com/user-attachments/assets/cd7cc59d-45b5-4ef8-baed-ccb728ba37d5" />
- Promoted the server to a Domain Controller and created the marc.local domain for centralized user authentication.

5. <img width="1080" height="1080" alt="AD Users Group OU" src="https://github.com/user-attachments/assets/92ae93ba-ea06-4fde-a4a7-15e785456ecd" />
- Created organizational units, users, and security groups to simulate a basic company structure within Active Directory.

6. <img width="1351" height="685" alt="Domain and New User in Domain" src="https://github.com/user-attachments/assets/b61e3455-9ef7-49ff-8f1c-774f0178c55a" />
- Successfully joined a Windows 11 client machine to the marc.local Active Directory domain and authenticated using domain user accounts.




Issues Encountered
- The virtual machine initially failed to boot into the Windows Server installer because the incorrect ISO file was attached. This was resolved by downloading and mounting the correct Windows Server ISO.
- Network connectivity between CLIENT01 and DC01 initially failed because both virtual machines were on different subnets. This was resolved by reconfiguring both VMs to use the same Host-only virtual network.
- CLIENT01 received a 169.254.x.x APIPA address after switching networks, indicating DHCP failure. A manual IPv4 configuration was applied to place the client in the same subnet as the domain controller.
- Ping requests initially failed due to Windows Firewall restrictions on DC01. ICMP Echo Request inbound rules were enabled to allow connectivity testing between virtual machines.
- Domain name resolution issues occurred because the client machine was not initially configured to use the domain controller as its DNS server. This was resolved by manually setting the preferred DNS server to 192.168.10.10.


Skills Demonstrated
- Windows Server installation
- Active Directory setup
- User and group management
- Domain controller configuration
- Basic DNS troubleshooting
- Technical documentation
