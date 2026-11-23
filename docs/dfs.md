[← Back to Main README](../README.md)

# Distributed File System (DFS) & Replication

Distributed File System (DFS) provides a unified namespace for shared enterprise folders and keeps data synchronized across both servers using **DFS Replication (DFSR)**.

## Implementation Highlights

- Configured a centralized **DFS Namespace** so clients access shared folders through a consistent logical path independent of the underlying server.
- Enabled **DFS Replication (DFSR)** between the two Windows Server instances for automatic folder synchronization and storage redundancy.
- Verified synchronized shared data folders on both server contexts.

## Verification Screenshots

**DFS Namespace**

![DFS Namespace](../screenshots/06-dfs-namespace.png)

**DFS Replication**

![DFS Replication](../screenshots/07-dfs-replication.png)

**Primary Server Shared Data Folders**

![Server Data Folders](../screenshots/13-server-data-folders.png)

**Additional Server Synchronized Data**

![ADC Server Data](../screenshots/16-adc-server-data.png)
