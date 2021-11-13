# BananaPi M2 Pro
This repository contains intallation script for the Banana Pi M2 Pro SBC.

## Base image
Base image for this installation is
> 2021-06-21-debian-10-buster-bpi-m5-m2pro-aarch64-sd-emmc.img
from vendor website.

## What does script do?
1. Rename host to "BananaPi";
2. Upgrade system;
3. Make user pi as sudo;
4. Add another users (specify name of them or comment it);
5. Install Banana Pi Tools;
6. Install Bluetooth Driver;
7. Install Network Manager (for manage Wi-Fi);
8. Install Desktop Environment (LXQt or XFCE);
	Desktop is LightDM (displat manager) + xfwm (window mananger) + LXQt/XFCE;
	LightDM is configured to provide user list on logon screen and autologin for pi user
9. Install Wi-Fi & Bluetooth utils (Network Manager Gnome and Blueman);
10. Install and configure VNC (TigerVNC) for :0 (physical) and :1 (pi) displays;
11. Install other userful apps (comment unnecessary or add your favorite);
12. Make some system changes;
	1) Add user "pi" to group "bluetooth";
	2) Change HDMI mode to 720p;
	3) Enable Network Manager for managing network adapters
13. Reboot.
