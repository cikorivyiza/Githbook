# Creating MBR Partitions

**`gdisk /dev/sda :`**` ``is used to launch the GPT (GUID Partition Table) fdisk utility for the disk device /dev/sda. GPT is a partitioning scheme used on modern disks that provides advantages over the older MBR (Master Boot Record) partitioning scheme, such as support for larger disk sizes and more partitions.`

**`lsblk`**` ``: list block devices`&#x20;

**`fdisk /dev/sdb`**` ``: open a window to create partitions in an assisted mode`

**`partprobe :`**` ``used to inform the Linux kernel about changes to the partition table of a disk without requiring a system reboot`

**`cat /proc/partitions`**` ``command displays information about the partitions on your system's disks`

