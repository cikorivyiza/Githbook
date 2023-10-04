# Understanding the NTP Protocol

<figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

In the Network Time Protocol (NTP), "**stratum**" represents the hierarchical level of time servers. **Stratum 0** refers to precise reference clocks like atomic clocks. **Stratum 1** servers sync with **Stratum 0** sources, serving as highly accurate time servers. **Stratum 2** servers synchronize with **Stratum 1** servers, and this hierarchy can continue with **Stratum 3, 4,** and so on till to **startum 16**. Lower stratum levels indicate greater accuracy, making **Stratum 1** servers the most trusted sources for time synchronization in NTP networks.
