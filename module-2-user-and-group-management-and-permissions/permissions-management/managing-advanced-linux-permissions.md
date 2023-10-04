# Managing Advanced Linux Permissions

**`chmod u+s playme`**` ``: it allows any user who runs that file to execute it with the permissions of the file's owner, rather than with their own permissions. This can be useful for certain programs that need elevated privileges to perform specific tasks.`

**`find / -perm /4000 :`**`  ``is used to search the entire filesystem  for files with the SUID (Set User ID) or SGID (Set Group ID) permissions set.`&#x20;

**`chmod g+s /data/account/ :`**` ``When the SGID permission is set on a directory, any new files or subdirectories created within that directory inherit the group ownership of the parent directory, rather than the group ownership of the user who created them. This can be useful in situations where you want all files within a directory to have a consistent group ownership.`

**`chmod +t /data/account/`**` ``: sets the stickybit on the directory, When the sticky bit is set on a directory, it means that only the owners of files within that directory can delete those files, even if other users have write permissions on the directory. This is often used on shared directories, like /tmp, to prevent files from being deleted by users other than their owners`
