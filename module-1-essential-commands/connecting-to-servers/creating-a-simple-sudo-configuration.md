# Creating a simple sudo configuration

**sudo visudo** : used to edit the sudoers file on Unix-based systems, typically Linux. The sudoers file controls who is allowed to run commands with superuser (root) privileges using the `sudo` command.



<details>

<summary>Understanding the folder /etc/sudoers.d/</summary>

In addition to the main sudoers file, which is typically located at `/etc/sudoers`, many Unix-like operating systems also support including additional configuration files from the `/etc/sudoers.d/` directory. This directory is used to organize and manage sudoers rules in a more modular and manageable way, especially in environments with multiple administrators or where you want to separate different configuration files for different purposes.

Here's how it works:

1. **Directory Structure**: The `/etc/sudoers.d/` directory contains multiple files, each with its own set of sudoers rules. These files should have no file extension and should follow a specific naming convention, such as `01_custom_rules`, `02_admin_rules`, etc. The numbers in the filenames determine the order in which these files are read, with lower numbers being processed first.
2. **Modularity**: Using this directory structure allows you to break down your sudoers configuration into smaller, more manageable files. For example, you could have one file for custom rules, one for specific user privileges, and another for group privileges.
3. **Avoiding Conflicts**: The `/etc/sudoers` file is typically maintained by the system and can be overwritten during system updates. By using `/etc/sudoers.d/`, you can add your custom rules and configurations without directly modifying the main sudoers file. This helps prevent conflicts during system updates.
4. **Syntax**: The syntax for the rules in these files is the same as in the main sudoers file. Each line defines a user, group, host, command, and privilege level. Be sure to follow the same syntax and rules as you would in the main sudoers file.

Here's an example of how you might use the `/etc/sudoers.d/` directory:

```
// # Create a new sudoers file in /etc/sudoers.d/
sudo visudo -f /etc/sudoers.d/custom_rules

# Add your custom sudoers rules to the /etc/sudoers.d/custom_rules file
# For example, allow the user 'myuser' to run 'some_command' with sudo
myuser ALL=(ALL) NOPASSWD: /path/to/some_command
```

</details>
