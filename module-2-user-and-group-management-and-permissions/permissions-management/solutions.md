# Solutions

*   **umask 077 :**&#x20;

    The command `umask`` `**`077`** sets the umask for the current user's session to **077**. The umask is a permission mask that determines the default permissions assigned to newly created files and directories.

    In this case, with a umask of 077:

    * New files will have permissions 600, which means they are readable and writable by the owner but not accessible to others.
    * New directories will have permissions 700, which means they are accessible only to the owner, and others have no permissions.

    To make this persistant you have to write in the file **.baschrc** and **.bashrc\_profile**



* **mkdir - /data/sales /data/account :**&#x20;

