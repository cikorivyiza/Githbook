# Understanding Targets



* A target is a group of services&#x20;
* Some targets are isolatable, which means that you can use them as a state your system should be in
  * emergency.target&#x20;
  * rescue target&#x20;
  * multi-user.target&#x20;
  * graphical.target
* Use **`systemctl list-dependencies name.target`** to see the contents and dependencies of a systemd target

