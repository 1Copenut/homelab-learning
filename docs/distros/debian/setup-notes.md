# Debian links
I like Debian. Maybe server-only. Maybe a daily driver. Maybe just a VM.

## Setup and Hardening
- [Set up and auto-mount Ethernet cards](https://www.youtube.com/watch?v=X1HyrSzmtKA)
- [Securing Debian Manual](https://www.debian.org/doc/manuals/securing-debian-manual/security-update.en.html)

## BIOS
- [Updating the Lenovo Thinkpad BIOS in Linux and Ubuntu Environments](https://www.youtube.com/watch?v=2CGrawsd_TA&t=5s)
- [How to update Lenovo BIOS from Linux without using Windows](https://www.cyberciti.biz/faq/update-lenovo-bios-from-linux-usb-stick-pen/)

### DHCP
* Release DHCP lease. Helpful when moving from dynamic to static IP
  ```shell
  # Use the MAC address to target this NIC in static IP
  # assignment, then release and renew the dhclient
  sudo dhclient -r # releases current DHCP lease
  sudo dhclient # re-enables dhclient with new lease
  ```
