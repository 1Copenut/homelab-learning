# Debian links
I like Debian. Maybe server-only. Maybe a daily driver. Maybe just a VM.

## Setup and Hardening
- [Set up and auto-mount Ethernet cards](https://www.youtube.com/watch?v=X1HyrSzmtKA)

### DHCP
* Release DHCP lease. Helpful when moving from dynamic to static IP
  ```shell
  # Use the MAC address to target this NIC in static IP
  # assignment, then release and renew the dhclient
  sudo dhclient -r # releases current DHCP lease
  sudo dhclient # re-enables dhclient with new lease
  ```
