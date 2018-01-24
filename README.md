# Rando-Scripto
Script to be used on Ubuntu images during CyberPatriot competitions. Created in 2016. Ongoing project.


Usage
-----
Open the terminal and log in to superuser by running the following:
```shell
sudo su
```
It will prompt you to enter your password.

After entering your password, run the following line:
```shell
chmod +x Script
```
It sets the permission for the script to be executable.

To run the script itself, run the following line:
```shell
./Script
```

IMPORTANT: DO NOT RUN THE TEST SCRIPT!
--------------------------------------
IT IS USED AS A BACKUP FOR WHATEVER I'M CURRENTLY WORKING ON. IT CONTAINS LINES OF CODE THAT IS STILL BEING TESTED. MOST OF THE CODE WILL THROW A LOT OF ERROR MESSAGES AND IT IS **POSSIBLE** THAT IT CONTAINS CODE THAT WILL RENDER YOUR MACHINE UNUSABLE.

The Test Script is currently set to skip the entirety of its code. If you really want to see the terminal filled with a bunch of unnessary error messages, remove ": <<'SKIP'" and "SKIP" from the code and run it.


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
      - The script will only automatically enable ufw and automatically run chkrootkit and bastille. The rest is up to user discretion
  - Setting some permissions.
  - Open some files that are important to the CyberPatriot competition. Can be ignored. Just keep hitting the 'x' button in the top left corner.


Things It Don't Do (In the order it is not performed)
-----------------------------------------------------
  - Remove the sketchy programs and media file extensions. That is up to the user, just in case you want to keep some of them on your system.
  - Get you all those points in CyberPatriot competitions.
  - Make you a good script writer. Seriously. I probably need to rewrite this because it's pretty poorly written.
  
  
Future Updates
--------------
  - Add an option that allows user to choose to perform a system update now or wait until later.
  - Allow for user to set their own default password or use "Goodpassword123!"
      - Will also add an option to not change current user's password to the default.


Contributors
------------
@MrAsian, @DrDavid52
