# using fdisk

My fdisk is in /sbin/fdisk

My fdisk is fdisk from util-linux 2.33.1

usage seems to be fdisk [options]

## lowercase option flags

`fdisk -b` requires argument. used to specify the sector size in bytes  when using the fdisk command-line utility for partitioning storage devices.

`fdisk -c` says bad usage. this is not actually a command.

`fdisk -h` prints help. Displays help information about the usage of fdisk. This is useful for quickly getting a reminder of the available commands and options.

`fdisk -l` lists disks and needs sudo perms. this lists the partitions. `sudo fdisk -l` Lists all the disks and their partitions. This operation typically requires superuser permissions (sudo). It's a quick way to see the current state of disk partitions.

`fdisk -o` says option requires an argument

`fdisk -s` says bad usage. this is not actually a command. Provides the size of a partition in blocks. This option can be handy for quickly assessing the capacity of individual partitions.

`fdisk -t` says option requires an argument. allows you to change the type of an existing partition on your storage device `sudo fdisk -t /dev/sdX type_code`

`fdisk -u` says bad usage. This flag alters the display units when listing partition tables, showing sizes in sectors instead of cylinders. This can be particularly useful for precise measurements and calculations involving disk space.

`fdisk -v` prints the version

`fdisk -w` says option requires an argument. used to write the changes you've made to the partition table on your storage device `sudo fdisk -w /dev/sdX`.  Writes the changes made to the partition table to the storage device. Like many other operations in fdisk, this requires an argument specifying the target device and typically requires superuser permissions.

## uppercase flags

`fdisk -B` says bad usage

`fdisk -C` says option requires an argument. Sets the number of cylinders on the disk. Adjusting this parameter can be necessary for certain disk configurations or when dealing with older hardware.

`fdisk -H` says option requires an argument. Specifies the number of heads on the disk. Similar to -C, this option is more relevant to older disk geometries.

`fdisk -L` says bad usage

`fdisk -S` says option requires an argument. Defines the number of sectors per track on the disk. This option is another relic from the era of physical disk geometry definitions.

`fdisk -V` prints the version

`fdisk -W` says option requires an argument

Help is at fdisk --help and also you can `man fdisk`
