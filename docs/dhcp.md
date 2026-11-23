[← Back to Main README](../README.md)

# Dynamic Host Configuration Protocol (DHCP)

The DHCP Server role manages dynamic IPv4 address allocation, scope options (default gateway and DNS servers), lease renewals, and client access policies across the lab network.

## Implementation Highlights

- Configured centralized DHCP scopes to automatically assign IP configurations to domain Windows clients.
- Tested and verified dynamic lease allocation and client-side `ipconfig /release` and `ipconfig /renew` workflows.
- Configured DHCP client restrictions/filters to control lease assignment behavior.
- Integrated DHCP with high-availability failover (see [DHCP Failover](dhcp-failover.md)).

## Verification Screenshots

- **Server Role Configuration:** ![PDC Server Manager](../screenshots/01-pdc-server-manager.png)
- **Client IP Allocation:** ![DHCP Client IP Allocation](../screenshots/04-dhcp-client-ip-allocation.png)
- **Release & Renew Test:** ![DHCP Release and Renew](../screenshots/05-dhcp-release-renew.png)
- **Client Restrictions:** ![DHCP Client Restrictions](../screenshots/20-dhcp-client-restrictions.png)
- **Client & Server Verification:** ![DHCP Client Server Data](../screenshots/21-dhcp-client-server-data.png)
