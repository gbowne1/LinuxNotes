# How to configure a filesystem

I am writing this as a means to set up a bootable disk with filesystem on Debian based linux with available tools especially command line.

## Bootable USB 2.0 key

I will attempt to make a bootable USB 2.0 key.

### Device


### Main partition

- description: EXT4 volume
- logical name: /dev/sd*
- size: 2GiB
- vendor: Linux
- capacity: 2GiB
- capabilities primary bootable journaled extended_attributes large_files huge_files dir_nlink 64bit extents ext4 ext2 initialized
- configuration:

### Swap Partition

- logical name: /dev/sd
- size: 2GiB
- capacity: 2GiB
- capabilities: primary swap initialized

## Bootable SSD

## Bootable spinning disk

description: ATA Disk
product:
physical id:
bus info: scsi@
logical name: /dev/sd*
version:
serial:
size:
capabilities: gpt-1.00 partitioned partitioned:gpt
configuration: ansiversion=5 guid=<guid> logicalsectorsize=512 sectorsize=512
