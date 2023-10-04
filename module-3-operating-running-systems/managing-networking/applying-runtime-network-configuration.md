# Applying runtime network configuration

**`ip a`**` ``: shows the current network configurations`

**`ip route show`**` ``: shows the current route configurations`

**`cat /etc/resolv.conf :`**` ``shows the ip of the DNS`

**`ip route del default via 192.168.4.2 :`**` ``deletes the default route`&#x20;

**`ip route add default via 192.168.4.2`**` ``: adds the default route`&#x20;

**`ip add del dev ens33 192.168.4.245/24`**` ``: deletes the ip on dev ens33`

**`ip addr add dev ens33 192.168.4.245/24 :`**` ``adds the ip on dev ens33`

**`dhclient :`**` ``sends a DHCP discover packet to the network, requesting an IP address and other network configuration information.`

