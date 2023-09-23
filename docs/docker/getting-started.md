# Getting started on Docker
I like Docker for running complex apps in containers. I also like Debian because I've been building containers in Debian for a few months. So this article and following articles will assume Debian 12 (Bookworm) or newer as the starting point.

## Installing the Debian `iso`
* Grabbed the offical [64 bit PC netinst iso](https://www.debian.org/distrib/) from Debian's website
* Grabbed the `SHA256` [checksum](https://cdimage.debian.org/debian-cd/current/amd64/bt-dvd/). Had to dig for the answer, but it's in the ISO's parent directory.
* Created the `root` and daily user. Strong passwords for both. **In password manager** this time.
* `su -` to elevate privilege
* `apt update` and `apt upgrade`
* Create Proxmox backup (optional). Could opt to wait until after Docker is installed.

### Adding a QEMU agent
I haven't started doing much with [QEMU guest agents](https://pve.proxmox.com/wiki/Qemu-guest-agent) so far, but I'm making it a point to install them on all VMs I create. As fate would have it, I forgot to install it on the Debian VM, but it was pretty easy to add after the fact:

* Click on the VM, then click `Options` in Proxmox web GUI
* Click on `QEMU Agent` and then click `Edit`
* Check the box for `Use QEMU Guest Agent` and click `OK`
* QEMU agent will run the next time you start the VM

## Installing and verifying Docker
* Watched the excellent video [How To Install Docker In A Proxmox VM](https://www.youtube.com/watch?v=xCWEmHW_uE4) by Tech Tutorials (David McKone)
* Read the associated blog post by the same name to get the [commands to copy/paste](https://www.techtutorials.tv/sections/docker/how-to-install-docker/) into Debian terminal
* `su DOCKER_USER` to test the Docker install
* `docker run hello-world`
* Verify the success message works
* Backup the Debian VM in Proxmox and watch sportsball before stating the next task
