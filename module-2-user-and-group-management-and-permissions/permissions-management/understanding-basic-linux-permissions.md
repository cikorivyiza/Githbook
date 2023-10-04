# Understanding Basic Linux Permissions

In Linux Permissions are assigned to **UGO** : Users,Groups and Others.

1. We use **chown** to change **user owner** and **chgrp** to change **group owner**
2. Permission mode is a way to define which permission are going to be applied to a file and we use **chmod** for this stuf, we can use the absolute mode or relative mode
   1. i.e : **chmod **<mark style="color:red;">**761 file**</mark>

|                                                        | FILE                                                  | DIR                                                          |
| ------------------------------------------------------ | ----------------------------------------------------- | ------------------------------------------------------------ |
| Read equal to <mark style="color:red;">**4**</mark>    | Open equal to <mark style="color:red;">**4**</mark>   | List equal to <mark style="color:red;">**4**</mark>          |
| Write equal to <mark style="color:red;">**2**</mark>   | Modify equal to <mark style="color:red;">**2**</mark> | Create/Delete equal to <mark style="color:red;">**2**</mark> |
| Execute equal to <mark style="color:red;">**1**</mark> | Run equal to <mark style="color:red;">**1**</mark>    | cd equal to <mark style="color:red;">**1**</mark>            |

