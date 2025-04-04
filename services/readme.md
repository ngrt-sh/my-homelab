# Service

## Docker stack
In my Docker cluster, they are some many apps that runs inside. One VM is dedicated for a specific usage such as multimedia, networking and file sharing.

Below they are by hosts the containers I run and her running case

### apollo (VM)
Docker cluster -- Main node management with Portainer
- Portainer
- Immich
- Plex

### heimdall (VM)
Docker cluster -- Node slave with Portainer agent
- Portainer Agent
- Nginx Proxy Manager
- AdGuard Home
- WireGuard VPN

### chronos (host)
Docker cluster -- Node slave with Portainer agent
 - Portainer Agent
 - UptimeKuma
 - Duplicati

## Virtual machine stack
![vm_stack]()
