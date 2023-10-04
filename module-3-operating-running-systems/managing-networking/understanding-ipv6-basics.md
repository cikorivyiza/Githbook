# Understanding IPv6 Basics



### IPv6 Addresses

* Addresses are 128 bits and written in hexadecimal
  * **fe80:1223:3345:5567:abcd:efef:1000:0001**
* Leading zeros can be omitted, as well as long strings of zeros •&#x20;
  * **fe80::1**
* When referring to address + port, put the address between square brackets:&#x20;
  * **\[fe80::1]**
* Default subnet mask is **/64**&#x20;
* Node bit of the address may contain the device MAC address



### Reserved Addresses

* **::128**      localhost&#x20;
* **::**           unspecified address (0.0.0.0)&#x20;
* **::/0**          default route&#x20;
* **2000::/3**       global unicast address&#x20;
* **fd00::/8**        unique local address (private addresses)&#x20;
* **fe80::/64** link-local address&#x20;
* **ff00::/8**         multicast



### Obtaining an IPv6 Address

* **fe80::** address is used by default&#x20;
* Through static addressing&#x20;
* DHCPv6 Multicast is sent out to ff02::1:2 port 547/UDP. This is the all-DHCP multicast group. The DHCP server sends a packet back to client 546/UDP&#x20;
* SLAAC (Stateless Address Auto Configuration) Router solicitation is sent to ff02::2; the all-routers multicast group. The router sends back an IP address, which allows the host to learn the network prefix. Install the radvd package to use this
