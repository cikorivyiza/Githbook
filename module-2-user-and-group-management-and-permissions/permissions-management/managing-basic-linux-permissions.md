# Managing Basic Linux Permissions

**Absolute mode :**&#x20;

**`chmod 770 account/ :`**` ``sets the "account" file or directory to be readable, writable, and executable by the owner and the group but not accessible at all by others.`

**Relative mode :**&#x20;

**`chmod g+W account/ :`**` ``adds write permission for the group to the "account" directory.`

**`chmod g-w account/ :`**` ``removes write permission for the group from the "account" directory.`

**`chown anna account`**` ``: used to change the ownership of a file or directory named "account" to the user "anna" in a Unix-like operating system.`

**`chown anna:account account/`**` ``: is used to change both the owner and group ownership of the "account" directory to the user "`**`anna`**`" and the group "`**`account`**`".`
