# Managing umask

* The **umask** is a Shell setting that defines a mask that will be subtracted from the default permissions&#x20;
* Default permissions on directories are **777**
* &#x20;Default permissions on files are **666**&#x20;
  * **umask 022** will set default permissions on files to **644**&#x20;
  * **umask 027** will set default permissions on directories to **750**
*
