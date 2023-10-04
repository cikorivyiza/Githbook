# Using I/O Redirection and Piping

### Understanding Redirection

Redirection is used to manipulate input and output of commands&#x20;

* Standard input(0):<
  * **sort \</etc/services :** sort the content of etc/passwd
* Standard Output&#x20;
  * **ls>\~/myfile :** Creates a file named "myfile" in your home directory that contains the listing of files and directories from the current directory.
  * **who>>\~myfile :** the output of the `who` command will be appended to the "myfile" file, preserving any existing content in that file.
  * **sort \</etc/passwd >somewhereelse :** the contents of the "/etc/passwd" file will be sorted, and the sorted result will be saved in the "somewhereelse" file. The original "/etc/passwd" file remains unchanged.
* Standard Error ():  >
  * **grep -R root /proc>/dev/null :**&#x20;
  * **grep -R root /etc &>\~/myfile :**&#x20;

#### Understanding Piping

* A pipe is used to send the output of one command to be used as input for a second command                &#x20;
  * **ps aux I grep http**
* The **tee** command combines redirection and piping: It allows you to write output to somewhere, and at the same time use it as input for another command&#x20;
  * **ps aux I tee psfile I grep ssh** :&#x20;
  * **ps aux | tee file | grep ssh** : gives a list of processes that include "ssh" in their details, and this list will be both displayed on your terminal and saved to a file named "file" in the current directory.

