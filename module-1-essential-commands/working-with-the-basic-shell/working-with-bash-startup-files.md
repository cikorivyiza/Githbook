# Working with Bash Startup Files

* **/etc/environment** contains a list of variables and is the first file that is processed while starting bash (empty by default on Red Hat)&#x20;
*   /etc/profile is executed while users login&#x20;

    * **/etc/profile.d** is used as a snapin directory that contains additional configuration
    * **\~/.bash\_profile** can be used as a user-specific version&#x20;
    * **\~/.bash\_logout** is processed when a user logs out&#x20;


* **/etc/bashrc** is processed every time asubshell is started&#x20;
  * A user specific **\~/.bashrc** file may be used
