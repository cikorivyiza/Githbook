# Working with grep

We can use grep in  two ways

1. **ps aux | grep ssh** : shows a list of process then filters ssh using grep
2. **grep amy  /etc/\*** : looks for files where the text amy is present
3. **grep amy  /etc/\*  2>/dev/null :** looks for files where the text amy is present and redirects erros to the null device

{% hint style="info" %}
In linux everything is case sensitive
{% endhint %}

## Options

1. **grep hello demofile** : dump to the screen all matching lines that contains the word hello in the file demofile
2. **grep -i hello demofile** : dump to the screen all matching lines that contains the word hello in the file demofile without taking in account case sensitivity of the word.&#x20;
3. **ps aux | grep ssh | grep -v grep :** list all processes related to SSH by filtering the output of the ps aux command and then excluding lines that contain the string "grep," which is used for the previous grep command itself. This way, you'll get a clean list of SSH-related processes.
4. **grep -R root \*** : will search through all files in the current directory and its subdirectories for lines containing the word "root" and display the matching lines along with the filenames where the matches were found.
5. **grep -R root \* -l :** search through all files in the current directory and its subdirectories for the word "root" and will display the filenames of the files that contain this pattern.



