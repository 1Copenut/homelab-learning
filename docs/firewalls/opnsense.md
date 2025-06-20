# OPNSense
I didn't like where pfSense was going in terms of licensing and user information required to use the community version, so I'm looking closer at OPNSense now.

* [Virtualize OPNsense on Proxmox as Your Primary Router](https://homenetworkguy.com/how-to/virtualize-opnsense-on-proxmox-as-your-primary-router/)

## Configuration

### Disks
* [FreeBSD: Adding Disks](https://docs.freebsd.org/en/books/handbook/disks/#disks-adding)
* [`mount`](https://man.freebsd.org/cgi/man.cgi?mount(8))
* [`fstab`](https://man.freebsd.org/cgi/man.cgi?fstab(5))

## Plugins and tools

### DNS (Unbound default)
* [Install Pi-hole on Proxmox and Use OPNsense Unbound DNS as Upstream DNS](https://homenetworkguy.com/how-to/install-pi-hole-on-proxmox-and-use-opnsense-unbound-dns-as-upstream-dns/) `verfied`

### Pihole
* [The big blocklist collection](https://firebog.net/)
* Change password from the container / Pihole commandline: `$ pihole -a -p`

## Traffic management (switches)
* [How to Configure VLANs on a TP-Link Managed Switch](https://homenetworkguy.com/how-to/configure-vlans-tp-link-switch/)
* [How to Configure VLANs on TP-Link Switch for UniFi Access Points with VLAN per SSID](https://homenetworkguy.com/how-to/configure-tp-link-switch-vlan-with-unifi-access-points-vlan-per-ssid/)
* [Set Up a Management VLAN for OPNsense, a Network Switch, and a Wireless Access Point](https://homenetworkguy.com/how-to/set-up-management-vlan-for-opnsense-network-switch-and-access-point/)

## Security

### Firewall rules
* [Drop versus Reject](https://www.chiark.greenend.org.uk/~peterb/network/drop-vs-reject)

