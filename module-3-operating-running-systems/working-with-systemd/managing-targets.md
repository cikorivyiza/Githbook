# Managing Targets

1. **`systemctl start name.target`**: Starts the systemd target named `name.target`.
2. **`systemctl isolate name.target`**: Switches to the specified systemd target, isolating it.
3. **`systemctl list-dependencies name.target`**: Lists dependencies of the systemd target `name.target`.
4. **`systemctl get-default`**: Displays the current default systemd target.
5. **`systemctl set-default name.target`**: Sets the default systemd target to `name.target`

