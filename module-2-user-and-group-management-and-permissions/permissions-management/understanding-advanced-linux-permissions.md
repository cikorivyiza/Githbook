# Understanding Advanced Linux Permissions



|                                                   | Files              | DIR                                              |
| ------------------------------------------------- | ------------------ | ------------------------------------------------ |
| SUID <mark style="color:red;">equal to 4</mark>   | Run as Owner       | N/A                                              |
| SGID <mark style="color:red;">equal to 2</mark>   | Run as group Owner | Inherit  directory group owner                   |
| Sticky <mark style="color:red;">equal to 1</mark> | N/A                | delete if you are owner of the dir or its parent |

To use these permissions we introduce a 4 digits permission such as&#x20;

chmod <mark style="color:red;">**4770**</mark>
