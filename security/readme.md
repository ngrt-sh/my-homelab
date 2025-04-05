# Security

I provide you how I manage in my homelab the security such as the update strategy, the usage of firewall, the authentication methods and how the backups are configured.

## Update strategy

My VMs (Debian, ...) and the Docker containers need to be manually updated, I don't have unattended updates setup. I update my system manually once time per month and same thing for the container.

## Firewall usage

I don't have (for the moment) any hardware firewall, so I'm obliged to install a firewall service and this is **fail2ban**. I just configured to fail2ban a SSH rules to prevent any bruteforce attacks inside my local network. The setup of fail2ban is incremental, so if the attacker attempt to bruteforce the SSH password three times, he will be in access denied during 10 minutes, 1 hour, 6 hours, 24 hours, 48 hours and finally to be blocked if during blocking it continues to force connection attempts.

## Authentication

To authenticate to my machines via SSH, for the moment I don't use the login keys and I will remain on the traditional passwords. For the web apps (Proxmox, TrueNAS, ...) I use the password authentication and I have added a two factor authentication method. I know this is useless in local but...

## Backup setup

Backuping data is very primordial whether for personal or business use. I have a 5 TB OneDrive account and I use the Duplicati software backup that runs inside a Docker container. Duplicati will backup on OneDrive automatically with scheduled backups.

### Devices used for storing my backups data
 - External 1.5 TB Western Digital Drive
   - Used for storing my Proxmox VM and Containers backups with a retention of 7 days, 4 weeks and 3 months to prevent the data saturation.

- Microsoft OneDrive 5 TB
  - Used for storing my backup of "everything" in my Homelab. How it scheduled :
    - 8:00 PM **Immich**
    - 9:30 PM **Musics**
    - 12:00 AM **NAS Data**
    - 3:00 AM **Proxmox VM and CT**
   
- External 1 TB Drive
  - Used for the externalization of my data. The disk will remain all the school days in my high school locker. The weekend and holidays he will remains at my home to keep safe and update it every sundays with the most recent backups.
