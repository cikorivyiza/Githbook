# Understanding Users and Groups Configuration Files

For centralised authentication users and groups informations are stored in 4 files which are :&#x20;

* **/etc/passwd :**&#x20;
  * Purpose: This file stores user account information.
  * Content: Each line in the file represents a user account and contains fields like username, encrypted password (historically stored here, but now usually in `/etc/shadow`), user ID (UID), group ID (GID), user's full name, home directory, and the default shell.
  * Access: Typically, it is readable by all users on the system but should not be writable by regular users.
* **/etc/shadow :**&#x20;
  * Purpose: This file enhances security by storing user password hashes and other account security settings.
  * Content: It contains fields like username, password hash (encrypted password), password expiration information, account lockout information, and more.
  * Access: It is usually only readable by the superuser (root) to prevent unauthorized access to sensitive password data.
* **/etc/group :**&#x20;
  * Purpose: This file stores information about user groups.
  * Content: Each line in the file represents a group and contains fields like group name, group password (rarely used), group ID (GID), and a list of user names that are members of the group.
  * Access: Typically, it is readable by all users on the system but should not be writable by regular users.
* **/etc/gshadow :**&#x20;
  * Purpose: This file enhances security for group management by storing group password hashes and other group-related security settings.
  * Content: Similar to `/etc/shadow`, it contains fields like group name, encrypted group password, and administrative information related to group management.
  * Access: Like `/etc/shadow`, it is usually only readable by the superuser (root) for security reasons.

1. **`vipw`**`: Safely edit the /etc/passwd file for user account information, locking it to prevent concurrent edits and performing checks before updating.`
2. **`vipw -s`**`: Securely edit the /etc/shadow file, storing user password hashes and security info, with file locking and integrity checks.`
3. **`vigr`**`: Safely edit the /etc/group file, which stores user group information, while preventing concurrent edits and ensuring proper formatting.`
