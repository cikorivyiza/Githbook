---
description: a.k.a Globbing in official documentation
---

# Using wildcards

Wildcards in a linux file system allows you to refere to a file in a flexible way&#x20;

* **`ls *`**` ``= unlimited number of characters`
  * `ie : if you type`` `**`ls *`**` ``you will see all files names in current directory`
  * **`ls a*`**` ``: shows files with an`` `**`a`**` ``at the begining followed by anything`
  * **`ls *a`**` ``: shows files with an`` `**`a`**` ``at the end`
  * **`ls -d a?s* :`**` ``shows an`` `**`a`**` ``on the first position, second position doesn't matter, third position must be an`` `**`s`**
  * **`ls -d a[lm]*`**` ``: shows an`` `**`a`**` ``on the first position, second position must be a letter between`` `**`l`**` ``and`` `**`m.`**
  * **`ls -d a[l-m]*`**` ``: shows an`` `**`a`**` ``on the first position, second position must be a letter in the range between`` `**`l`**` ``and`` `**`m.`**
* **`ls ?`**` ``= single character`
* **`ls [a-d]`**` ``= a range betwen a and d`

You can also combine them :

* **`ls [a-c]* :`**` ``all files with a name starting with an a,b or c.`
* **`ls ?[z-s]*`**` ``: all files with a name where the`` `**`2nd character`**` ``is  with an z`` `**`or`**` ``an`` `**`s`**

The -d option is used for ignoring the content of directories.

