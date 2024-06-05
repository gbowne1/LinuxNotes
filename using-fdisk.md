# using fdisk

My fdisk is in /sbin/fdisk

My fdisk is fdisk from util-linux 2.33.1

usage seems to be fdisk [options]

## lowercase option flags

`fdisk -b` requires argument. used to specify the sector size in bytes  when using the fdisk command-line utility for partitioning storage devices

`fdisk -c` says bad usage. this is not actually a command.

`fdisk -h` prints help

`fdisk -l` lists disks and needs sudo perms. this lists the partitions. `sudo fdisk -l`

`fdisk -o` says option requires an argument

`fdisk -s` says bad usage. this is not actually a command.

`fdisk -t` says option requires an argument. allows you to change the type of an existing partition on your storage device `sudo fdisk -t /dev/sdX type_code`

`fdisk -u` says bad usage

`fdisk -v` prints the version

`fdisk -w` says option requires an argument. used to write the changes you've made to the partition table on your storage device `sudo fdisk -w /dev/sdX`

## uppercase flags

`fdisk -B` says bad usage

`fdisk -C` says option requires an argument

`fdisk -H` says option requires an argument

`fdisk -L` says bad usage

`fdisk -S` says option requires an argument

`fdisk -V` prints the version

`fdisk -W` says option requires an argument

Help is at fdisk --help and also you can `man fdisk`
