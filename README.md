# Ubuntu-Hardening-1
Script to be used on Ubuntu images during CyberPatriot competitions. Created in 2016. Ongoing project.

This is an outdated version of the scripte. Go [here](https://github.com/MrAsian/Ubuntu-Hardening-2) for the updated and revised version of the script.

Usage
-----
Open the terminal and log in to superuser by running the following:
```bash
sudo su
```
It will prompt you to enter your password. After entering your password, navigate to where the script is store and enter the following command to run it.
```bash
bash ./Script
```


Things It Do (In the order it is performed)
-------------------------------------------
  - List all possible sketchy programs and media file extensions that should be removed on user's discretion. This list of programs and media file extensions only include CyberPatriot's usual list of point giving programs and file extensions.
      - Sketchy programs include:
          apache2, bind9, cain, cracklib, hydra, john, nc, netcat, nginx, postgresql, samba, telnet, tftp-server, vsftpd
      - Media file extensions include:
          .jpg, .mp3, .mp4, .png
  - Sets a default password on ALL users, including the current user.
      - The default password is "Goodpassword123!" without the quotes, in case you get locked out.
  - Some STIG viewer things. Some work, some don't. Will probably be removed.
      - Red Hat Enterprise Linux 6 STIGs
      - Oracle Linux 6 STIGs
  - Require authentication to access sudo.
  - Disable Guest account
  - Configure secure settings on SSH.
      - Root account cannot be logged onto from SSH
      - SSH will be set to use port 222
  - Configure password policy.
      - Password min length will be set to 12
      - Retry attempts will be set to 3
      - Password max age will be set to 60
      - Password min age will be set to 59
  - Disable IPv6
  - System Update
  - Install some useful security programs.
      - Useful Security Programs include:
          apparmor, bastille, chkrootkit, clamav, lynis, rkhunter, ufw
      - The script will only automatically enable ufw and automatically run chkrootkit and bastille. Whether to use or enable the rest is up to user discretion.
  - Setting some permissions.
  - Open some files that are important to the CyberPatriot competition. Can be ignored. Just keep hitting the 'x' button in the top left corner of the files that pop up. Or use the escape sequence "ctrl + c" to terminate the script.


Contributors
------------
@MrAsian, @DrDavid52
