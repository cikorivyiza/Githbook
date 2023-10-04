# Managing Linux Time

**`date`**` ``: print the current date and time in the default format`

**`date -s`**` ``: it will change the system's date and time accordingly. For example, date -s "2023-10-02 14:30:00"`

**`hwclock -s`**` ``: used to set the hardware (RTC - Real-Time Clock) clock from the system time`

**`hwclock -w`**` ``: command is used to write the system time to the hardware clock. This ensures that the hardware clock is updated to match the current system time.`

**`timedatectl`**` ``: used to query and control system time and date settings.`

**`timedatectl list-timezones`**` ``: It provides a list of timezone identifiers that you can use with the`` `**`timedatectl set-timezone`**` ``command.`

**`timedatectl set-timezone Europe/AMsterdam`**` ``: This command is used to set the system's timezone to a specific timezone. In this example, it sets the timezone to "`**`Europe/Amsterdam"`**

**`timectl status`**` ``: This command displays detailed information about the system's current date and time settings, including the timezone, current time, time synchronization status, and more`
