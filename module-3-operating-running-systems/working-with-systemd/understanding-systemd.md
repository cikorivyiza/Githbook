# Understanding Systemd

* Systemd is the manager of everything&#x20;
* It's the first thing that is started after starting the Linux kernel&#x20;
* It starts processes and can do that in parallel&#x20;
* It also manages mounts, timers, paths, and much more&#x20;
* It is event driven, which means that it can react to specific events
* The items that are managed by systemd are called units&#x20;
* Default units are in **/usr/lib/systemd/**system, custom units are in **/etc/systemd**
