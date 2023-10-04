# Understanding Network Device Naming

biosdevname uses device names that reveal information about physical location, and **systemd-udevd** generates the network device names

* em123 (Ethernet Motherboard Portnumber)&#x20;
* p\<port>p\<slot> (PCI, PCI port)&#x20;
* eno123 (EtherNet Onboard)&#x20;
* If driver doesn't reveal sufficient information, etho etc. is used
