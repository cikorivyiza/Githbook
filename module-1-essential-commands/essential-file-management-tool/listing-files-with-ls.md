---
description: List directory contents
layout: landing
---

# Listing Files with ls

When you type ls -l in the terminal you get this result

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

From the right to the left the columns are respectively :thumbsup:

1. _**Name**_ of the file of the directory
2. Creation _**date**_ of the file
3. The _**size**_ of the file in kb
4. _**Permissions**_ related to the file : _**user + group**_ who _**owns**_ the file
5. _**link counter**_
6. _**Permissions**_ _**set**_ to the file in 3 groups : _**user owner,group owner and others**_, it's because linux permissions applies to those 3 groups

The first Character _**d**_ or _**l**_ is the indicator of the type of the file it stands for _**directory**_ or _**symbolic link**_

Options for ls

* _**`ls -a`**_` ``: shows hidden files`
* _**`ls -lrt`**_` ``: list files by showing the last modified in last`
* _**`ls -l  / home`**_` ``: shows the content of the directory`
* _**`ls -ld  / home`**_` ``: shows the properties of the directory`

