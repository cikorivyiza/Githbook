# Modifying Service Configuration

* **`systemctl cat name.service`**` ``reads current unit configuration`&#x20;
* **`systemctl show`**` ``shows all available configuration parameters`&#x20;
* **`systemctl edit name.service`**` ``allows you to edit service configuration`&#x20;
* `After modifying service configuration, use`` `**`systemctl daemon-reload`**&#x20;
* `Next, use`` `**`systemctl restart name.service`**` ``to restart the service`
