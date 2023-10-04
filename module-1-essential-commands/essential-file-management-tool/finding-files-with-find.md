# Finding files with find

**`find / -name "hosts"`**` ``: look at files that exists in / which is root directory based on the exact name hosts`

**`find / -user amy`**` ``: search for files and directories on the system where the owner is the user named "amy." This command starts the search from the root directory ("/") and recursively searches through the entire file system`

**`mkdir /root/amy; find / -user amy -exec cp {} /root/amy \;`**` ``: create the "amy" directory under "/root" and then search for files and directories owned by the user "amy" on your system, copying them into the "/root/amy" directory.`

**`find / -size +100M`**` ``:`&#x20;

**`find / -size +100M 2>/dev/null`**` ``: search the entire file system for files larger than 100 megabytes and display a list of those files while suppressing any error messages. This can be useful for identifying large files on your system`

**`mkdir -p files/new; cp /etc/hosts files/new :`**` ``run two commands immediately`
