# Monitoring and managed alerts

Here this is how I can monitoring and how the alerts are managed my homelab if something went wrong. There is not much because most of the time it is just a container and bash scripts that are there.

# Used monitoring tools

First, for the monitoring by simple ping on the network, I use the [UptimeKuma](https://github.com/louislam/uptime-kuma) container wich is deployed in my Raspberry Pi. I have added all the possible sensors that I need such as, the network devices, the VM and CT on my Proxmox, the containers also some DNS servers like Cloudflare DNS, Quad9.

Also, I have maked a bash script on my Proxmox wich is runned every minutes and the bash script will ping my monitoring Raspberry Pi in case if he crash.

I have also added some sensors like a CPU temperature, SMART anomally detection, long intensive CPU usage or a high usage memory.

*Note: these scripts will be available soon in a dedicated repo. Stay tuned!*

# How alerts are configured

All my alerts are centralized the a Discord webhook notification system.

![webhook](https://github.com/ngrt-sh/my-homelab/blob/main/monitoring/2025-04-06_18-24.png?raw=true)
