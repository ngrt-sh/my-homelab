# Infrastrucure

## Diagram of my complete local network

![network](https://github.com/ngrt-sh/my-homelab/blob/main/infrastructure/complete_infra.png?raw=true)

## Hosts

Here, I show you all my physical/virtual machines and containers that run into my homelab, her roles and why I use it.

### Physical machines

| Machine | Inside hardware                      | OS                                   | Use case                                                                                |
|---------|--------------------------------------|--------------------------------------|-----------------------------------------------------------------------------------------|
| atlas   | - Asus OEM Motherboard               | Debian 12 with Proxmox VE packages   | For virtualize my applications in VMs with separed usages                               |
|         | - Intel Core i5-3330 4C 4T @ 3.00 GHz|                                      |                                                                                         |
|         | - 16 GB of RAM DDR3                  |                                      |                                                                                         |
|         | - 250 GB SSD (boot)                  |                                      |                                                                                         |
|         | - x4 1 TB HDD                        |                                      |                                                                                         |
| chronos | Raspberry Pi 4                       | DietPi (Debian based)                | For infra monitoring and daily backup into the cloud. Part of my Docker cluster.        |

### Virtual Machines

| Machine | VM hardware                          | OS                                   | Use case                                                                                                                                                                            |
|---------|--------------------------------------|--------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| apollo  | - 4C CPU                             | Debian 12                            | The master of my Docker cluster. Used for multimedia taks such as storing and streaming musics and also storing and streaming my photo and videos like a self-hosted Google Photos. |
|         | - 4 GB of RAM                        |                                      |                                                                                                                                                                                     |
|         | - 32 GB boot SSD                     |                                      |                                                                                                                                                                                     |
|         | - x2 1 TB HDD (VM passtrought)       |                                      |                                                                                                                                                                                     |
| heimdall| - 4C CPU                             | Debian 12                            | The second node of my Docker cluster. Used for network tasks such as VPN, reverse proxy and VPN.                                                                                    |
|         | - 4 GB of RAM                        |                                      |                                                                                                                                                                                     |
|         | - 16 GB boot SSD                     |                                      |                                                                                                                                                                                     |
| truenas | - 2C CPU                             | TrueNAS SCALE 24.10 (Debian 12 based)| Used for SMB and NFS shares inside my local network.                                                                                                                                |
|         | - 2 GB of RAM                        |                                      |                                                                                                                                                                                     |
|         | - 16 GB boot SSD                     |                                      |                                                                                                                                                                                     |

### Containers (Proxmox)

| Machine      | VM hardware                          | OS                                   | Use case                                                                                                                                                                       |
|--------------|--------------------------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| nexus        | - 4C CPU                             | Debian 12                            | Used for storing my website/portfolio.                                                                                                                                         |
|              | - 256 MB of RAM                      |                                      |                                                                                                                                                                                |
|              | - 8 GB boot SSD                      |                                      |                                                                                                                                                                                |
| cerbere      | - 4C CPU                             | Debian 12                            | Used for my second DNS.                                                                                                                                                        |
|              | - 512 MB of RAM                      |                                      |                                                                                                                                                                                |
|              | - 8 GB boot SSD                      |                                      |                                                                                                                                                                                |
| nexus-dev    | - 4C CPU                             | Debian 12                            | Used for the developpement part of my website/portfolio.                                                                                                                       |
|              | - 512 MB of RAM                      |                                      |                                                                                                                                                                                |
|              | - 8 GB boot SSD                      |                                      |                                                                                                                                                                                |
| bots-discord | - 4C CPU                             | Debian 12                            | Used for hosting my discord bots.                                                                                                                                              |
|              | - 512 MB of RAM                      |                                      |                                                                                                                                                                                |
|              | - 8 GB boot SSD                      |                                      |                                                                                                                                                                                |
| static       | - 4C CPU                             | Debian 12                            | Used for storing some static files for my website.                                                                                                                             |
|              | - 512 MB of RAM                      |                                      |                                                                                                                                                                                |
|              | - 8 GB boot SSD                      |                                      |                                                                                                                                                                                |
