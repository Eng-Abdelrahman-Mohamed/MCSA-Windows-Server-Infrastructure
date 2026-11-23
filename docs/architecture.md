[← Back to Main README](../README.md)

# Architecture

This Windows Server 2019 lab was built in **VMware Workstation** to simulate an enterprise domain environment with directory services, name resolution, high-availability IP addressing, distributed file services, centralized security policies, and remote VPN access.

The environment includes **two Domain Controllers** (Primary Domain Controller and Additional Domain Controller) along with Windows client machines used for configuration testing and end-to-end validation.

## Logical Architecture

```text
                 Windows Server 2019 Infrastructure
              (Primary DC & Additional DC in VMware)
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
   Active Directory       DNS               DHCP / Failover
   (AD DS / OUs)     (Name Resolution)  (Redundant IP Leases)
        │                                     │
        └────────────── Windows Clients ──────┘

        File Services / DFS  ── Shared Storage & Replication (DFSR)
        Group Policy (GPO)   ── Centralized Endpoint Security
        RRAS / VPN           ── Remote Access & Cross-Subnet Routing
```

## Role-to-Screenshot Map

| Area | Verification Captures |
|---|---|
| Primary server roles | [01-pdc-server-manager.png](../screenshots/01-pdc-server-manager.png) |
| Directory & Domain Controllers | [02-active-directory-ous-users.png](../screenshots/02-active-directory-ous-users.png), [12-pdc-this-pc.png](../screenshots/12-pdc-this-pc.png), [14-adc-active-directory-users.png](../screenshots/14-adc-active-directory-users.png), [15-adc-this-pc.png](../screenshots/15-adc-this-pc.png) |
| DHCP & Failover | [03-dhcp-failover.png](../screenshots/03-dhcp-failover.png), [04-dhcp-client-ip-allocation.png](../screenshots/04-dhcp-client-ip-allocation.png), [05-dhcp-release-renew.png](../screenshots/05-dhcp-release-renew.png), [17-dhcp-failover.png](../screenshots/17-dhcp-failover.png), [20-dhcp-client-restrictions.png](../screenshots/20-dhcp-client-restrictions.png), [21-dhcp-client-server-data.png](../screenshots/21-dhcp-client-server-data.png) |
| DFS & Shared Folders | [06-dfs-namespace.png](../screenshots/06-dfs-namespace.png), [07-dfs-replication.png](../screenshots/07-dfs-replication.png), [13-server-data-folders.png](../screenshots/13-server-data-folders.png), [16-adc-server-data.png](../screenshots/16-adc-server-data.png) |
| Group Policy | [08-group-policy-management.png](../screenshots/08-group-policy-management.png), [09-gpo-security-validation.png.png](../screenshots/09-gpo-security-validation.png.png) |
| RRAS / VPN & Routing | [10-vpn-server-active-client.png](../screenshots/10-vpn-server-active-client.png), [11-vpn-client-routing-test.png](../screenshots/11-vpn-client-routing-test.png), [18-vpn-server-manager.png](../screenshots/18-vpn-server-manager.png), [19-vpn-client-ipconfig.png](../screenshots/19-vpn-client-ipconfig.png) |
