# Common Text Processing Utilities

**cut : f**ilter output from a text file

**sort :** sort files, often used in pipes

**tr :** translates uppercase to lowercase

**awk :** search for specific patterns

**sed :** powerful stream editor to batch-modify text files



Examples

**cut -d : -f 1 /etc/passwd | sort** : When you run this command, it will output a list of usernames from the `/etc/passwd` file, with each username on a separate line,&#x20;

**-d :** is the option for the delimiter, the file /etc/passwd is delimited by :&#x20;

**-f 1** : is another option that specifies the first field to extract .



**echo hello | tr \[:lower:] \[:upper:]** : translate the word hello to HELLO&#x20;



**sed -n 5p /etc/passwd** : prints the 5th line of the file /etc/passwd

**sed -i s/how/HOW/g myfile :** modifies interactively the word how to HOW in the file myfile.

**sed -i -e '2d' myfile** : deletes the 2nd line in myfile



**awk -F : '{ print $4}' /etc/passwd | sort -n :** extract the fourth field (which is typically the user's UID or user ID) from each line, and then sorts those values numerically

**awk -F : '/amy/ { print $4 } ' /etc/passwd** : uses the `awk` command to search for lines in the `/etc/passwd` file that contain the string "amy" and then prints the fourth field (typically the user's UID) from those lines



