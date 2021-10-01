# Kali_RPi_RIAB
This is a HOWTO and scripts for turning a RaspberryPi 2/3/4 into a Cyber Range In A Box (RIAB).. or, a portable, headless, penetration box that can both function as an autonomous sniffer, or as a WiFi to Ethernet NAT firewall, which you can use from either your terminal or via Remote Desktop, either over WiFi or secure, wired connection.  
![image](https://raw.githubusercontent.com/Tweeks-va/Kali_RPi_RIAB/main/RAIB-Desc.png)

The live, cloud slides for this demo talk are located here - https://vacr.io/bsides-kali

hackroute - A post-boot run-once script that fixes the eth0 issue of our static 192.168.168.168 "server IP" not coming up.. it also ensures that wlan0 comes up, and that all traffic gets routed through the Eth-->WiFi NAT we set up using iptables and sysctl (kernel) forwarding. It's ugly.. but it seems to work (after disabling NetworkManager and enabling networking.service). Should be enabled via /etc/rc.local or the like.

All of my related materials and code are copy left (open sourced) under the Creative Commons (CC)(BY)(NC)(SA)[1] License.

[1] - https://en.wikipedia.org/wiki/Creative_Commons_license#Types_of_licenses
