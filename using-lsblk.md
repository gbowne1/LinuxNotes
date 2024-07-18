# using lsblk

The lsblk command is a versatile tool used in Unix-like operating systems to list information about all available or the specified block devices. Block devices represent storage devices such as hard drives, SSDs, and removable media like USB flash drives.

`lsblk -a` used to list all block devices.  includes loop devices?

`lsblk -b`. May not actually exist

`lsblk -d` lists information in a `distinguishing` state

`lsblk -e` displays info about all block devices including those not mounted

`lsblk -f` displayed info in a `full` format.  shows uuid, mountpoin, label, fstype,

`lsblk -h` displays info in a human readable format

`lsblk -i` displays detailed information with focus on I/O capabilities

`lsblk -l` displays all information including their attributes

`lsblk -m` shows permissions

`lsblk -n` May not actually exist, but still returns

`lsblk -o` requires an argument.  Not a standard option flag.  but can be used to customize output by FIELD. `lsblk -o NAME,SIZE`

`lsblk -p` lists information by their physical path

`lsblk -r`

`lsblk -s`

`lsblk -t`

`lsblk -x` requires an argument

`lsblk -z` lists zones
