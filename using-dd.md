# using dd

Besides being called universal disk destroyer, it can be pretty useful.

This particular command does not use upper or lowercase flags or options.

## dd options

if= Input file. Specifies the input file or device.

of= Output file. Specifies the output file or device.

bs= Block size. Sets the block size for reading and writing.

count= Number of blocks to copy. Limits the number of bytes copied.

skip= Number of blocks to skip at the beginning of the input file.

seek= Number of blocks to seek ahead in the output file.

status= Controls the progress reporting. Can be set to none, progress, or process.

conv= Conversion options. Useful for byte swapping or text encoding.

iflag= Input and output flags. Control how dd reads from and writes to files/devices.

oflag= Input and output flags. Control how dd reads from and writes to files/devices.

ibs= Input and output block sizes. Different from bs when dealing with multibyte characters.

obs= Input and output block sizes. Different from bs when dealing with multibyte characters.

noerror= Continue on read errors. Ignores errors encountered during the copy process

notrunc= Do not truncate the output file. Preserves existing data in the output file.

sync= Synchronize I/O operations. Ensures that all data is written before exiting.

progress= Show progress bar. Provides visual feedback on the progress of the operation.

nocreat=  Do not create the output file if it does not exist. Only truncates it.

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
