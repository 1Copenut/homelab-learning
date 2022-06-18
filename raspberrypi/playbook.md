# Raspberry Pi provisioning
This file will ultimately become a playbook for provisioning Raspberry Pis more quickly and efficiently.

## Steps
1. Flash a new image
2. `$ touch ssh` to the boot volume to enable SSH
3. Power up and create custom user (this may have to be changed for playbook automation)
4. `$ passwd` to create a stronger password
5. `$ sudo apt-get update && sudo apt-get upgrade`
6. Change hostname using `$ sudo raspi-config`
7. Disable passwordless root access
8. Set root password
9. Disable root login
10. Create SSH key for daily driver
11. Copy SSH key to Pi, test connection
12. Remove password login `$ sudo vi /etc/ssh/sshd_config` and look for `#PasswordAuthentication no`
13. Install ufw or iptables
14. Set the firewall to accept only SSH traffic (22 or other if changed), HTTP/S (80, 443)
15. Install Fail2ban
16. Adjust Fail2ban policy for aggressive bans
17. Disable Bluetooth
18. Disable WiFi if using a hardline connection (recommended)
19. Install software as needed
