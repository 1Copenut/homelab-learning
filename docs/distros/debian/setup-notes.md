# Debian (and Debian-like) links
I like Debian. Maybe server-only. Maybe a daily driver. Maybe just a VM. I also like Ubuntu and Mint. Will be including those here because they're derived from Debian.

## Setup and Hardening
- [Set up and auto-mount Ethernet cards](https://www.youtube.com/watch?v=X1HyrSzmtKA)
- [Securing Debian Manual](https://www.debian.org/doc/manuals/securing-debian-manual/security-update.en.html)

## BIOS
- [Updating the Lenovo Thinkpad BIOS in Linux and Ubuntu Environments](https://www.youtube.com/watch?v=2CGrawsd_TA&t=5s)
- [How to update Lenovo BIOS from Linux without using Windows](https://www.cyberciti.biz/faq/update-lenovo-bios-from-linux-usb-stick-pen/)

## Virtualizaztion
- [How to Install KVM on Ubuntu 24.04: Step-By-Step](https://www.cherryservers.com/blog/install-kvm-ubuntu)
- [Setting Up Virtual Machines with QEMU, KVM, and Virt-Manager on Debian/Ubuntu](https://linuxconfig.org/setting-up-virtual-machines-with-qemu-kvm-and-virt-manager-on-debian-ubuntu)

### DHCP
* Release DHCP lease. Helpful when moving from dynamic to static IP
  
  ```shell
  # Use the MAC address to target this NIC in static IP
  # assignment, then release and renew the dhclient
  sudo dhclient -r # releases current DHCP lease
  sudo dhclient # re-enables dhclient with new lease
  ```
