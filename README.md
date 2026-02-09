# Active-Directory-Homelab
Active Directory lab built on Proxmox to practice real-world IT skills like domain management, DNS troubleshooting, Group Policy, and user/group administration.

---

## Lab Overview
- Hypervisor: Proxmox VE (bare metal)
- Domain: 'lab.local'
- Servers and Clients:
  - Windows Server (Domain Controller + DNS) - 'DC01'
  - Windows 11 workstation (domain-joined)
-Networking
  - Single LAN subnet (domain DNS points to DC01)

---

## What I configured

### Active Directory Domain Services (AD DS)
- Created a new forest and domain: 'lab.local'
- Promoted 'DC01' to Domain Controller
- Built a custom OU structure (Users, Groups, Workstations, Servers, etc.)

### Users and Groups
- Created realistic user accounts
- Created security groups for role-based access (ex: Employees, HelpDesk, IT-Admins)
- Assigned users to groups based on role

### Group Policy
- Account Lockout Policy
- User restriction policy

### File and Permission Management
- Create a file share on DC01
- Configured share + NTFS permissions using security groups

---

## Skills Demonstrated
- Active Directory administration
- Group Policy creation + OU scoping
- Account lockout + unlock workflow
- Windows Server Administration + file share permissions
- Structured troubleshooting

---

## Screenshots

### Organizational Unit Structure
Designed a logical OU hierarchy to separate users, groups and administrative roles. 

![OU Structure](screenshots/01-ou-structure.png)

### Users and Security Groups
Created multiple users and role-based security groups to simulate a real environment

![Users and Groups](screenshots/02-users)(screenshots/03-groups)

