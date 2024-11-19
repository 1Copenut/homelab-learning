# Firewall rules
I usually end up writing the same basic rules right away (DNS, VLAN segmentation) and have to look them up every time.

## VLAN rules
These rules allow VLANs DNS access (default gateway) and internet access. They do not allow VLANs to see other VLANs' traffic.

| IP address | Protocol | Source | Source Port | Destination | Destination Port | Description |
| ---------- | -------- | ------ | ----------- | ----------- | ---------------- | ----------- |
| IPv4+6 | TCP, UDP | VLAN net | * | VLAN address | 53 | Allow access to DNS |
| IPv4 | * | VLAN net | * | !RFC1918 | * | Allow VLAN access to internet only |
