# Advanced options of find

**`find / -type f -size +100M`**` ``: search the entire file system and display a list of regular files that are larger than 100 megabytes in size`

**`find /etc -exec grep -l amy { } \ ; -exec cp { } root/amy/ \; 2>/dev/null :`**&#x20;

**`find /etc -name '*' -type f | xargs grep "127.0.0.1"`**

**`find /etc/ -type f -size -1000c -exec cp {} /tmp/files/pictures/ ;`**` ``: find files under the /etc/ directory that are smaller than 1000 bytes and then copy them to /tmp/files/pictures/.`

