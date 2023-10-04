# Copying Files with cp

Typically we copy a source file to a destination but if we are copying to a directory we can have multiple sources.

ie :&#x20;

* **`cp /etc/hosts .`**` ``: copy hosts in the current directory`
* **`cp -R /tmp .`**` ``: Recursive copy that copy the entire contents of the "/tmp" directory, including subdirectories and their contents.`

Sometimes it's good to put a **/** at the end of the command if you're copying a directory to be sure.

