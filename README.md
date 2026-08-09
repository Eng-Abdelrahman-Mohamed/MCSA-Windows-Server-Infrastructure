# MCSA Windows Server Infrastructure Lab

> A practical Windows Server infrastructure lab built in VMware Workstation and documented through 21 screenshots of the implemented environment.

<p align="center">
  <img src="https://img.shields.io/badge/VMware-Workstation-607078?style=for-the-badge&logo=vmware&logoColor=white" alt="VMware Workstation">
  <img src="https://img.shields.io/badge/Windows-Server-0078D4?style=for-the-badge&logo=windows&logoColor=white" alt="Windows Server">
  <img src="https://img.shields.io/badge/Active%20Directory-AD%20DS-5C2D91?style=for-the-badge" alt="Active Directory">
  <img src="https://img.shields.io/badge/DNS%20%7C%20DHCP-Network%20Services-2F80ED?style=for-the-badge" alt="DNS and DHCP">
  <img src="https://img.shields.io/badge/RRAS%20%7C%20VPN-Remote%20Access-333333?style=for-the-badge" alt="RRAS and VPN">
</p>

## Quick Navigation

- [Overview](#overview)
- [Objectives](#objectives)
- [Lab Environment](#lab-environment)
- [Technologies & Services](#technologies--services)
- [Infrastructure Overview](#infrastructure-overview)
- [Implemented Features](#implemented-features)
- [Testing & Verification](#testing--verification)
- [Evidence Gallery](#evidence-gallery)
- [Documentation](#documentation)
- [Repository Structure](#repository-structure)
- [Skills Demonstrated](#skills-demonstrated)
- [Author](#author)
- [Conclusion](#conclusion)

## Overview

This repository documents a hands-on Windows Server infrastructure lab. The screenshots are treated as the primary source of truth for the roles, services, administrative views, and validation activities represented in the project.

The project is a **training and portfolio lab** related to Windows Server/MCSA technologies. It does not claim an MCSA certification.

## Objectives

- Build and manage a Windows Server infrastructure in VMware Workstation.
- Configure and demonstrate directory, DNS, DHCP, file-service, policy, and remote-access functionality.
- Work with multiple server contexts and Windows client-side validation.
- Verify selected configuration and connectivity workflows using administrative tools and client tests.
- Document the implemented work in a clear, evidence-based format.

## Lab Environment

| Component | Evidence-based description |
|---|---|
| Virtualization | VMware Workstation |
| Server platform | Windows Server |
| Server contexts | PDC and ADC are visibly referenced in the screenshots |
| Client systems | Windows client-side configuration and validation views are present |

Exact Windows versions, VM count, hardware resources, IP ranges, domain name, and complete topology are **Not confirmed from the available evidence.**

## Technologies & Services

| Technology | Purpose | Evidence |
|---|---|---|
| Active Directory Domain Services | Directory and identity management | [01](screenshots/01-pdc-server-manager.png) · [02](screenshots/02-active-directory-ous-users.png) · [14](screenshots/14-adc-active-directory-users.png) |
| DNS | Server-side name-service role | [01](screenshots/01-pdc-server-manager.png) |
| DHCP | Dynamic client addressing | [04](screenshots/04-dhcp-client-ip-allocation.png) · [05](screenshots/05-dhcp-release-renew.png) |
| DHCP Failover | DHCP failover administration | [03](screenshots/03-dhcp-failover.png) · [17](screenshots/17-dhcp-failover.png) |
| DFS Namespace | Namespace administration | [06](screenshots/06-dfs-namespace.png) |
| DFS Replication | Replication administration | [07](screenshots/07-dfs-replication.png) |
| Group Policy | GPO management and validation | [08](screenshots/08-group-policy-management.png) · [09](screenshots/09-gpo-security-validation.png.png) |
| RRAS / VPN | Remote-access and routing activity | [10](screenshots/10-vpn-server-active-client.png) · [11](screenshots/11-vpn-client-routing-test.png) · [18](screenshots/18-vpn-server-manager.png) |
| File & Storage Services | Server/data-folder evidence | [01](screenshots/01-pdc-server-manager.png) · [13](screenshots/13-server-data-folders.png) · [16](screenshots/16-adc-server-data.png) |

Exact configuration values, protocols, IP addresses, credentials, commands, and several test outcomes are **Not confirmed from the available evidence.**

## Infrastructure Overview

The evidence supports a Windows Server lab containing directory services, DNS, DHCP, DFS, Group Policy, file/data services, and RRAS/VPN-related activity, with client-side validation screens.

A high-level evidence-based view is documented in [Architecture](docs/architecture.md).

> **Important:** the architecture documentation intentionally avoids inventing IP addresses, hostnames, routes, server counts, or topology details that are not established by the screenshots.

## Implemented Features

- Windows Server role and service administration through Server Manager.
- Active Directory OU and user-management activity.
- DNS role visibility.
- DHCP client IP allocation and release/renew activity.
- DHCP client restrictions and client/server DHCP-related views.
- DHCP failover views.
- DFS Namespace and DFS Replication administration.
- Group Policy management and security validation.
- RRAS/VPN server and client activity.
- Client routing/connectivity testing.
- Server and client system/data-folder verification.

## Testing & Verification

Validation activities are documented in [Testing & Verification](docs/testing.md), including:

- DHCP allocation and release/renew workflows
- DHCP failover views
- DHCP client restrictions
- Group Policy validation
- VPN/RRAS activity
- Client routing testing
- DFS and server data evidence
- Active Directory and system-information verification

Where a screenshot does not clearly establish an exact result or value, the documentation states **Not confirmed from the available evidence.**

## Evidence Gallery

All 21 screenshots are displayed directly below as visual evidence. The original filenames are preserved.

### Server & Active Directory

**PDC Server Manager**  
*Windows Server roles and services visible in the lab.*

![PDC Server Manager](screenshots/01-pdc-server-manager.png)

**Active Directory OUs and Users**  
*Active Directory organizational units and user-management view.*

![Active Directory OUs and Users](screenshots/02-active-directory-ous-users.png)

**PDC System View**  
*PDC system information view.*

![PDC System View](screenshots/12-pdc-this-pc.png)

**Server Data Folders**  
*Server-side data folders visible in the lab.*

![Server Data Folders](screenshots/13-server-data-folders.png)

**ADC Active Directory Users**  
*ADC Active Directory users view.*

![ADC Active Directory Users](screenshots/14-adc-active-directory-users.png)

**ADC System View**  
*ADC system information view.*

![ADC System View](screenshots/15-adc-this-pc.png)

**ADC Server Data**  
*ADC server-side data view.*

![ADC Server Data](screenshots/16-adc-server-data.png)

### DHCP & Failover

**DHCP Failover**  
*DHCP failover administration view.*

![DHCP Failover](screenshots/03-dhcp-failover.png)

**DHCP Client IP Allocation**  
*Client-side IP allocation evidence.*

![DHCP Client IP Allocation](screenshots/04-dhcp-client-ip-allocation.png)

**DHCP Release and Renew**  
*DHCP release and renew workflow evidence.*

![DHCP Release and Renew](screenshots/05-dhcp-release-renew.png)

**DHCP Failover — Additional View**  
*Additional DHCP failover administration view.*

![DHCP Failover Additional View](screenshots/17-dhcp-failover.png)

**DHCP Client Restrictions**  
*DHCP client restriction configuration/evidence view.*

![DHCP Client Restrictions](screenshots/20-dhcp-client-restrictions.png)

**DHCP Client / Server Data**  
*DHCP client/server data and validation view.*

![DHCP Client Server Data](screenshots/21-dhcp-client-server-data.png)

### DFS

**DFS Namespace**  
*DFS Namespace administration view.*

![DFS Namespace](screenshots/06-dfs-namespace.png)

**DFS Replication**  
*DFS Replication administration view.*

![DFS Replication](screenshots/07-dfs-replication.png)

### Group Policy

**Group Policy Management**  
*Group Policy Management view.*

![Group Policy Management](screenshots/08-group-policy-management.png)

**GPO Security Validation**  
*GPO security validation evidence.*

![GPO Security Validation](screenshots/09-gpo-security-validation.png.png)

### RRAS / VPN

**VPN Server and Active Client**  
*VPN/RRAS server view showing active-client related evidence.*

![VPN Server and Active Client](screenshots/10-vpn-server-active-client.png)

**VPN Client Routing Test**  
*Client-side routing/connectivity testing evidence.*

![VPN Client Routing Test](screenshots/11-vpn-client-routing-test.png)

**VPN Server Manager**  
*VPN/RRAS server management view.*

![VPN Server Manager](screenshots/18-vpn-server-manager.png)

**VPN Client IP Configuration**  
*VPN client IP configuration evidence.*

![VPN Client IP Configuration](screenshots/19-vpn-client-ipconfig.png)

## Documentation

| Document | Coverage |
|---|---|
| [Architecture](docs/architecture.md) | Evidence-based logical infrastructure overview |
| [Active Directory](docs/active-directory.md) | AD DS, OUs, and user-management evidence |
| [DNS](docs/dns.md) | DNS role evidence and confirmed limitations |
| [DHCP](docs/dhcp.md) | Address allocation and DHCP client/server activity |
| [DHCP Failover](docs/dhcp-failover.md) | DHCP failover evidence |
| [DFS](docs/dfs.md) | DFS Namespace, Replication, and data evidence |
| [Group Policy](docs/group-policy.md) | GPO management and validation |
| [RRAS / VPN](docs/rras-vpn.md) | VPN, remote access, and routing evidence |
| [Testing](docs/testing.md) | Consolidated testing and verification matrix |

## Repository Structure

```text
MCSA-Windows-Server-Infrastructure/
├── README.md
├── screenshots/
│   ├── 01-...
│   ├── 02-...
│   └── 21-...
└── docs/
    ├── architecture.md
    ├── active-directory.md
    ├── dns.md
    ├── dhcp.md
    ├── dhcp-failover.md
    ├── dfs.md
    ├── group-policy.md
    ├── rras-vpn.md
    └── testing.md
```

## Skills Demonstrated

- Windows Server administration
- Active Directory and OU/user management
- DNS and DHCP administration
- DHCP failover concepts and administration
- DFS Namespace and DFS Replication
- Group Policy management and validation
- RRAS / VPN and routing workflows
- Client/server troubleshooting and connectivity verification
- Technical documentation based on implementation evidence

## Author

**Abdelrahman Mohamed**  
Electrical Engineering Student | Telecommunications & Electronics

- 🔗 [LinkedIn](https://www.linkedin.com/in/abdelrahman-mhmed)
- 💻 [GitHub](https://github.com/Eng-Abdelrahman-Mohamed)

## Conclusion

This repository provides a structured portfolio record of a practical Windows Server infrastructure lab. The documentation focuses on what can actually be established from the 21 screenshots rather than filling gaps with assumed configurations.
