# using dd

Besides being called universal disk destroyer, it can be pretty useful.

This particular command does not use upper or lowercase flags or options.

## dd options

if=
of=
bs=
count=
skip=
seek=
status=
conv=
iflag=
oflag=
ibs=
obs=
noerror=
notrunc=
sync=
progress=
nocreat=

## Things you can do with dd

Copy a disk:           dd if=input_file of=output_file bs=1M

Cloning a disk:        sudo dd if=/dev/sdY of=/path/to/backup.img bs=4M status=progress

Wiping a disk:         sudo dd if=/dev/zero of=/dev/sdZ bs=4M status=progress

Making a boot USB:     sudo dd if=path/to/linux.iso of=/dev/sdX bs=4M status=progress

Copying a file:        dd if=input_file of=output_file bs=block_size

Byte order swap:       dd if=input.bin of=output.bin bs=4 conv=swab

Text encoder conv      dd if=ascii.txt of=ebcdic.txt conv=lcase,ebcdic-bcd

Back up MBR:           sudo dd if=/dev/sda of=mbr.bin bs=512 count=1

Making an ISO image:   sudo dd if=/dev/cdrom of=cd.iso bs=2048
