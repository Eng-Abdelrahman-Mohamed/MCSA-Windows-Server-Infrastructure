[← Back to Main README](../README.md)

# Testing and Verification Matrix

All core services across the Windows Server 2019 lab were tested and validated from both server management consoles and domain-joined client workstations.

| Verification Check | Screenshot(s) | Scope Covered |
|---|---|---|
| Server roles deployment | [01-pdc-server-manager.png](../screenshots/01-pdc-server-manager.png) | AD DS, DHCP, DNS, and File & Storage Services active on Primary DC |
| AD DS & OU structure | [02-active-directory-ous-users.png](../screenshots/02-active-directory-ous-users.png), [14-adc-active-directory-users.png](../screenshots/14-adc-active-directory-users.png) | Hierarchical OUs, users, and replication across Primary & Additional DCs |
| Server system properties | [12-pdc-this-pc.png](../screenshots/12-pdc-this-pc.png), [15-adc-this-pc.png](../screenshots/15-adc-this-pc.png) | Domain controller hostnames and system verification on both servers |
| DHCP Failover (Hot Standby) | [03-dhcp-failover.png](../screenshots/03-dhcp-failover.png), [17-dhcp-failover.png](../screenshots/17-dhcp-failover.png) | Active DHCP failover relationship and scope synchronization |
| DHCP client lease allocation | [04-dhcp-client-ip-allocation.png](../screenshots/04-dhcp-client-ip-allocation.png) | Dynamic IPv4 lease, gateway, and DNS assignment on Windows client |
| DHCP release / renew | [05-dhcp-release-renew.png](../screenshots/05-dhcp-release-renew.png) | End-to-end client lease release and renewal validation |
| DHCP client restrictions | [20-dhcp-client-restrictions.png](../screenshots/20-dhcp-client-restrictions.png), [21-dhcp-client-server-data.png](../screenshots/21-dhcp-client-server-data.png) | DHCP client policy enforcement and server/client data checks |
| DFS Namespace & Replication | [06-dfs-namespace.png](../screenshots/06-dfs-namespace.png), [07-dfs-replication.png](../screenshots/07-dfs-replication.png) | Unified DFS namespace and DFSR folder synchronization |
| Shared storage folders | [13-server-data-folders.png](../screenshots/13-server-data-folders.png), [16-adc-server-data.png](../screenshots/16-adc-server-data.png) | Synchronized shared data verification across both servers |
| Group Policy enforcement | [08-group-policy-management.png](../screenshots/08-group-policy-management.png), [09-gpo-security-validation.png.png](../screenshots/09-gpo-security-validation.png.png) | GPO creation, linking, and client-side security lockdown verification |
| RRAS / VPN & routing | [10-vpn-server-active-client.png](../screenshots/10-vpn-server-active-client.png), [11-vpn-client-routing-test.png](../screenshots/11-vpn-client-routing-test.png), [18-vpn-server-manager.png](../screenshots/18-vpn-server-manager.png), [19-vpn-client-ipconfig.png](../screenshots/19-vpn-client-ipconfig.png) | Active VPN tunnel, client IP addressing, and cross-subnet routing |
