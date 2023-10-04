# Using Common Network Tools

**`ping google.com`**` ``:`&#x20;

**`ping -f -s 4096 ubuntu`**` ``: will continuously send ICMP echo requests to the "ubuntu" host with 4096-byte packets without waiting for replies`

**`netstat -`**_**`tulpen`**_**` ``| less`**` ``: a paginated view of network-related information, including TCP and UDP connections, listening sockets, associated programs, and more`

**`ss -tuna`**` ``: almost equivalent to`` `**`netstat -`**_**`tulpen`**_

**`dig google.com`**` ``: used to query DNS servers and retrieve information about domain names`

**grep 68 /etc/services :** used to search for lines in the "**/etc/services**" file that contain the number "68" This file typically contains a list of **well-known service** names and their **associated port numbers** used by various network services on a Unix/Linux system.
