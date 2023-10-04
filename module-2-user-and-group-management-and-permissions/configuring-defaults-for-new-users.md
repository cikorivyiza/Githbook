# Configuring Defaults for New Users

* **useradd -D** can be used from the command line&#x20;
* /**etc/login.defs** is used as the default configuration file&#x20;
* **/etc/skell** contents is copied to user home directory upon user creation Linux does not offer an easy solution to apply new defaults to previously created users
* **/etc/default/useradd :** this file is used to set default parameters and options for the `useradd` command, which is used for adding new user accounts to the system.

**useradd -D :** The output will typically include information such as the default home directory format, default shell, default group, and other default user account settings.

