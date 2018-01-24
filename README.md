# Rando-Scripto
Script to be used on Ubuntu images during CyberPatriot competitions. Created in 2016. Ongoing project.

General Usage Notes
-------------------


THINGS IT DO (In the order it is performed)
-------------------------------------------
  - List all possible sketchy programs and media file extensions.
  - Sets a default password on ALL users, including the current user.
      - The default password is "Goodpassword123!" without the quotes, in case you get locked out.
  - Some STIG viewer things. Some work, some don't. Will probably be removed.
  - Require authentication to access sudo.
  - Disable Guest account
  - Configure secure settings on SSH.
  - Configure password policy.
  - Disable IPv6
  - System Update
  - Install some useful security programs.
  - Setting some permissions.
  - Open some files that are important to the CyberPatriot competition. Can be ignored, just keep hitting the 'x' button in the top left corner.


THINGS IT DON'T DO (In the order it is not performed)
-----------------------------------------------------
  - Remove the sketchy programs and media file extensions. That is up to the user, just in case you want to keep some of them on your system.
  - Get you all those points in CyberPatriot competitions.
  - Make you a good script writer. Seriously. I probably need to rewrite this because it's pretty poorly written.
  
  
FUTURE UPDATES
--------------
  - Add an option to perform a system update now or wait until later.
  - Add an option to install the security programs or skip the installation.
  - Allow for user to set their own default password or use "Goodpassword123!"
      - Will also add an option to not change current user's password.


CONTRIBUTORS
------------
MrAsian, DrDavid52
