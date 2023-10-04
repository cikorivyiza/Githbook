# Using ssh to Connect to a Remote Server

<figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption><p><em>ssh authentication process</em></p></figcaption></figure>



{% hint style="info" %}
the file **known\_hosts** located in .ssh contains the list of fignerprints of hosts we've connected to.
{% endhint %}

**ssh 192.168.32.2** : connect to the remote host 192.168.32.2 with ssh

**ssh 192.168.32.2 -X** : connect to the remote host 192.168.32.2 with ssh and gives the ability to open graphical applications.
