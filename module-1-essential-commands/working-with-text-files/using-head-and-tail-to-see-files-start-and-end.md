# Using head and tail to see Files start and end

**head /etc/passwd** : shows by default the first 10 lines of the file

**head -n 5 /etc/passwd** : shows 5 first line of the file passwd

**tail /etc/passwd** : shows by default the first 10 lines of the file

**tail -n 5 /etc/passwd** : shows 5 first line of the file passwd

**head -n 5 /etc/passwd | tail -n 1** : shows 5 first line and the last line of the file passwd

**tail -f /var/log/messages** : shows in real time what's happening in the log file
