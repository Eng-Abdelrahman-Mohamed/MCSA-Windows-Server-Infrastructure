# MCSA Windows Server Infrastructure Lab

> A practical Windows Server infrastructure lab built in VMware Workstation and documented through 21 screenshots of the implemented environment.

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

## Evidence Gallery

The gallery displays all 21 screenshots inline while preserving their exact filenames.

### Server & Active Directory\n\n![ PDC Server Manager ](screenshots/01-pdc-server-manager.png)\n\n*PDC Server Manager.*\n\n![ Active Directory OUs and Users ](screenshots/02-active-directory-ous-users.png)\n\n*Active Directory OUs and Users.*\n\n![ PDC system view ](screenshots/12-pdc-this-pc.png)\n\n*PDC system view.*\n\n![ Server data folders ](screenshots/13-server-data-folders.png)\n\n*Server data folders.*\n\n![ ADC Active Directory Users ](screenshots/14-adc-active-directory-users.png)\n\n*ADC Active Directory Users.*\n\n![ ADC system view ](screenshots/15-adc-this-pc.png)\n\n*ADC system view.*\n\n![ ADC server data ](screenshots/16-adc-server-data.png)\n\n*ADC server data.*\n\n### DHCP & Failover\n\n![ DHCP Failover ](screenshots/03-dhcp-failover.png)\n\n*DHCP Failover.*\n\n![ DHCP Client IP Allocation ](screenshots/04-dhcp-client-ip-allocation.png)\n\n*DHCP Client IP Allocation.*\n\n![ DHCP Release and Renew ](screenshots/05-dhcp-release-renew.png)\n\n*DHCP Release and Renew.*\n\n![ DHCP Failover — additional view ](screenshots/17-dhcp-failover.png)\n\n*DHCP Failover — additional view.*\n\n![ DHCP Client Restrictions ](screenshots/20-dhcp-client-restrictions.png)\n\n*DHCP Client Restrictions.*\n\n![ DHCP Client / Server Data ](screenshots/21-dhcp-client-server-data.png)\n\n*DHCP Client / Server Data.*\n\n### DFS\n\n![ DFS Namespace ](screenshots/06-dfs-namespace.png)\n\n*DFS Namespace.*\n\n![ DFS Replication ](screenshots/07-dfs-replication.png)\n\n*DFS Replication.*\n\n### Group Policy\n\n![ Group Policy Management ](screenshots/08-group-policy-management.png)\n\n*Group Policy Management.*\n\n![ GPO Security Validation ](screenshots/09-gpo-security-validation.png.png)\n\n*GPO Security Validation.*\n\n### RRAS / VPN\n\n![ VPN Server and Active Client ](screenshots/10-vpn-server-active-client.png)\n\n*VPN Server and Active Client.*\n\n![ VPN Client Routing Test ](screenshots/11-vpn-client-routing-test.png)\n\n*VPN Client Routing Test.*\n\n![ VPN Server Manager ](screenshots/18-vpn-server-manager.png)\n\n*VPN Server Manager.*\n\n![ VPN Client IP Configuration ](screenshots/19-vpn-client-ipconfig.png)\n\n*VPN Client IP Configuration.*\n\n## Repository Structure

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

## Conclusion

This repository provides a structured portfolio record of a practical Windows Server infrastructure lab. The documentation focuses on what can actually be established from the 21 screenshots rather than filling gaps with assumed configurations.
