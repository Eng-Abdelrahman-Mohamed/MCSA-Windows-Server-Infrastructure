# Architecture

This lab is presented as a VMware Workstation environment containing Windows Server systems and client-side validation screens. The screenshots establish a server/client infrastructure with directory services, name services, address assignment, file services, policy management, and remote-access testing.

The first screenshot visibly shows a VMware Workstation virtual machine named **PDC** with Server Manager displaying Active Directory Domain Services, DHCP, DNS, and File and Storage Services. Other screenshots show a second server context labelled **ADC** and client-side validation screens.

The exact number of virtual machines, network topology, IP ranges, default gateways, DNS zone names, hostnames beyond visible labels, and server-to-server links are **Not confirmed from the available evidence.**

## Logical View

The evidence supports the following high-level relationships:

```text
                 Windows Server Infrastructure
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
   Active Directory       DNS               DHCP
        │                  │                  │
   OUs / Users       Name services      Client addressing
        │                                     │
        └────────────── Windows Clients ──────┘

        File Services / DFS ── Shared data
        Group Policy        ── Policy management
        RRAS / VPN          ── Remote-access & routing activity
```

This is a conceptual evidence map, not a claim about the exact physical or virtual topology. Exact server links, IP addressing, routes, and service dependencies are **Not confirmed from the available evidence.**

## Evidence Map

| Area | Evidence |
|---|---|
| Primary server roles | [01-pdc-server-manager.png](../screenshots/01-pdc-server-manager.png) |
| Directory and client/server contexts | [02-active-directory-ous-users.png](../screenshots/02-active-directory-ous-users.png), [12-pdc-this-pc.png](../screenshots/12-pdc-this-pc.png), [14-adc-active-directory-users.png](../screenshots/14-adc-active-directory-users.png), [15-adc-this-pc.png](../screenshots/15-adc-this-pc.png) |
| DHCP and client addressing | [03-dhcp-failover.png](../screenshots/03-dhcp-failover.png), [04-dhcp-client-ip-allocation.png](../screenshots/04-dhcp-client-ip-allocation.png), [05-dhcp-release-renew.png](../screenshots/05-dhcp-release-renew.png), [17-dhcp-failover.png](../screenshots/17-dhcp-failover.png), [20-dhcp-client-restrictions.png](../screenshots/20-dhcp-client-restrictions.png), [21-dhcp-client-server-data.png](../screenshots/21-dhcp-client-server-data.png) |
| DFS and shared data | [06-dfs-namespace.png](../screenshots/06-dfs-namespace.png), [07-dfs-replication.png](../screenshots/07-dfs-replication.png), [13-server-data-folders.png](../screenshots/13-server-data-folders.png), [16-adc-server-data.png](../screenshots/16-adc-server-data.png) |
| Group Policy | [08-group-policy-management.png](../screenshots/08-group-policy-management.png), [09-gpo-security-validation.png.png](../screenshots/09-gpo-security-validation.png.png) |
| VPN/RRAS and routing | [10-vpn-server-active-client.png](../screenshots/10-vpn-server-active-client.png), [11-vpn-client-routing-test.png](../screenshots/11-vpn-client-routing-test.png), [18-vpn-server-manager.png](../screenshots/18-vpn-server-manager.png), [19-vpn-client-ipconfig.png](../screenshots/19-vpn-client-ipconfig.png) |
