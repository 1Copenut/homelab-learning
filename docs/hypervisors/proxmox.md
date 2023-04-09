# Proxmox Hypervisor Notes
I prefer a bare-metal hypervisor to a hosted one.

## Setup
* [How to Start a Home Lab: Part 1 - Proxmox VE](https://www.dlford.io/how-to-home-lab-part-1/)
* [How to Home Lab: Part 2 - Managing Proxmox VE](https://www.dlford.io/managing-proxmox-how-to-home-lab-part-2/)

## ZFS Storage
* [How to Install Proxmox and Setup a ZFS Pool](https://blog.quindorian.org/2019/08/how-to-install-proxmox-and-setup-a-zfs-pool.html/)
* [ZFS - Create Disk Pools](https://blog.programster.org/zfs-create-disk-pools)

## Hardening
Anything to make it harder to compromise a server.

###  SSH
* [Configuring SSH Fido U2F with Yubikey](https://lawrencesystems.com/configuring-ssh-fido-u2f-authentication-with-yubikey/)
* [SSH Copy ID](https://www.ssh.com/academy/ssh/copy-id) - to quickly copy the public key to a remote server
* [Fail2ban - Proxmox VE forums](https://pve.proxmox.com/wiki/Fail2ban)
* [Securing Proxmox and SSH using Fail2Ban](https://www.ukhost4u.com/securing-proxmox-and-ssh-using-fail2ban/)

## Automation
* [Provision Proxmox VMs with Ansible, quick and easy](https://vectops.com/2020/01/provision-proxmox-vms-with-ansible-quick-and-easy/)

## Troubleshooting
Anything that caused me grief or had to be looked up should go here.

### Networking
DNS, NIC configuration, VLANs, bridges, anything related to the flow of data should go here.

* [How to change my DNS settings](https://forum.proxmox.com/threads/how-to-change-my-dns.52879/)
* [Bring interfaces up after physical change](https://forum.proxmox.com/threads/network-interface-down-after-physical-change.70164/)
