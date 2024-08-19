# Configuration tips

## Display and general setup
* [Clock Format for Raspberry Pi Desktop](https://piwithvic.com/raspberry-pi-desktop-clock-format/)

## Security
Basic security procedures I should be undertaking while configuring new devices.

### SSH
* [How to Setup Raspberry Pi SSH Keys for Authentication](https://pimylifeup.com/raspberry-pi-ssh-keys/)
* [SSH with YubiKey FIDO U2F Authentication](https://forums.lawrencesystems.com/t/ssh-with-yubikey-fido-u2f-authentication/13024)

### Logging
* [Is Your Syslog Too big? Auto-rotate and automatically delete system log files.](https://medium.com/@nikhilbhanushali21/is-your-syslog-too-big-auto-rotate-and-automatically-delete-log-files-157b748f93d)
* [Why Should You Use the Gmail SMTP Server Method?](https://www.gmass.co/blog/gmail-smtp/)
* [Missing syslog file](https://forums.raspberrypi.com/viewtopic.php?t=358028)
* [ZRAM](https://github.com/ecdye/zram-config) - write to RAM and then to memory nightly. Saves writes to SD card.

### Monitoring
* `/usr/bin/vcgencmd measure_temp` to check CPU core temperature
