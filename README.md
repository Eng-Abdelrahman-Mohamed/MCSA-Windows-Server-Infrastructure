# MCSA Windows Server Infrastructure Lab

## Project Overview

This repository documents a practical Windows Server infrastructure lab built in VMware Workstation. The screenshots are the primary evidence for the services, configuration views, and validation activities represented here. This is a practical Windows Server/MCSA-related training project; it does not claim an MCSA certification.

## Objectives

- Configure and manage Windows Server roles and services.
- Demonstrate directory, address-management, file-services, policy, and remote-access functionality.
- Validate selected client/server and connectivity workflows through Windows administrative interfaces.

## Lab Environment

- VMware Workstation is visible in the evidence.
- Windows Server virtual machines are shown, including contexts labelled PDC and ADC.
- Client-side Windows configuration and validation screens are also present.

Exact Windows versions, VM count, hardware resources, IP ranges, domain name, and complete topology are **Not confirmed from the available evidence.**

## Technologies and Services

| Technology | Purpose | Evidence |
|---|---|---|
| Active Directory Domain Services | Directory and identity management | [Server role](screenshots/01-pdc-server-manager.png), [OU and users](screenshots/02-active-directory-ous-users.png) |
| DNS | Name-service role shown in Server Manager | [DNS role](screenshots/01-pdc-server-manager.png) |
| DHCP | Dynamic client addressing and validation | [Allocation](screenshots/04-dhcp-client-ip-allocation.png), [release/renew](screenshots/05-dhcp-release-renew.png) |
| DHCP Failover | Failover configuration/status views | [View 1](screenshots/03-dhcp-failover.png), [View 2](screenshots/17-dhcp-failover.png) |
| DFS Namespace | Namespace management | [DFS Namespace](screenshots/06-dfs-namespace.png) |
| DFS Replication | Replication management | [DFS Replication](screenshots/07-dfs-replication.png) |
| Group Policy | GPO management and validation | [Management](screenshots/08-group-policy-management.png), [validation](screenshots/09-gpo-security-validation.png.png) |
| RRAS/VPN | Server/client remote-access and routing evidence | [Server/client](screenshots/10-vpn-server-active-client.png), [routing test](screenshots/11-vpn-client-routing-test.png) |
| Server and file services | Server roles and data-folder views | [Server Manager](screenshots/01-pdc-server-manager.png), [data folders](screenshots/13-server-data-folders.png) |

Exact settings, protocols, addresses, credentials, and command outputs are **Not confirmed from the available evidence.**

## Infrastructure Overview

The evidence shows a Windows Server lab in VMware Workstation with at least two server contexts (PDC and ADC), client-side views, directory services, DHCP/DNS roles, DFS, Group Policy, and VPN/RRAS-related activity. A complete network diagram, exact server relationships, IP addressing plan, and topology are **Not confirmed from the available evidence.** See [architecture.md](docs/architecture.md).

## Implemented Services and Features

- Server Manager role visibility for AD DS, DHCP, DNS, and File and Storage Services.
- Active Directory OU and user-management activity.
- DHCP allocation, release/renew activity, restrictions, client/server data, and failover views.
- DFS Namespace and DFS Replication views.
- Group Policy management and security validation.
- VPN/RRAS server and client views, including routing-test evidence.
- Windows system and server data-folder verification.

## Testing and Verification

The evidence represents DHCP allocation and release/renew, DHCP failover views, Group Policy validation, VPN/RRAS activity, a routing-test view, and DFS/server data evidence. Definitive pass/fail results are recorded only where visible; otherwise they are **Not confirmed from the available evidence.** See [testing.md](docs/testing.md).

## Screenshot Evidence

All 21 screenshots remain at the repository root with their existing filenames.

- Core/server/AD: [01](screenshots/01-pdc-server-manager.png), [02](screenshots/02-active-directory-ous-users.png), [12](screenshots/12-pdc-this-pc.png), [13](screenshots/13-server-data-folders.png), [14](screenshots/14-adc-active-directory-users.png), [15](screenshots/15-adc-this-pc.png), [16](screenshots/16-adc-server-data.png)
- DHCP: [03](screenshots/03-dhcp-failover.png), [04](screenshots/04-dhcp-client-ip-allocation.png), [05](screenshots/05-dhcp-release-renew.png), [17](screenshots/17-dhcp-failover.png), [20](screenshots/20-dhcp-client-restrictions.png), [21](screenshots/21-dhcp-client-server-data.png)
- DFS: [06](screenshots/06-dfs-namespace.png), [07](screenshots/07-dfs-replication.png)
- Group Policy: [08](screenshots/08-group-policy-management.png), [09](screenshots/09-gpo-security-validation.png.png)
- VPN/RRAS: [10](screenshots/10-vpn-server-active-client.png), [11](screenshots/11-vpn-client-routing-test.png), [18](screenshots/18-vpn-server-manager.png), [19](screenshots/19-vpn-client-ipconfig.png)

## Repository Structure

- README.md
- docs/architecture.md
- docs/active-directory.md
- docs/dns.md
- docs/dhcp.md
- docs/dhcp-failover.md
- docs/dfs.md
- docs/group-policy.md
- docs/rras-vpn.md
- docs/testing.md
- configs/README.md
- 21 root-level PNG evidence files

## Skills Demonstrated

Windows Server administration; Active Directory and OU/user management; DHCP and DNS administration; DHCP failover; DFS Namespace and Replication; Group Policy administration and validation; VPN/RRAS and routing-test workflows; client/server troubleshooting and evidence-based verification.

## Conclusion

This repository presents a practical Windows Server infrastructure lab supported by 21 screenshots. It is a portfolio and training record of demonstrated administration tasks, not a certification claim.
