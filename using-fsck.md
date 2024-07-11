# using fsck

## lowercase flags

fsck from util-linux 2.33.1

fsck -a [auto] This option automatically repairs the file system without any questions (it's the same as -p)

fsck -b says Invalid non-numeric argument to -b ("dev/sde1"). This specifies the location of an alternate superblock to use for the file system check. The argument should be a number, not a device name.

fsck -c works "check for bad blocks". This option makes fsck check for bad blocks before doing the file system check.

fsck -d works "make no changes to filesystem". [debug]  This option makes fsck run in debug mode. It will show what's going on but make no changes to the file system.

fsck -f works "force check". [force] This forces fsck to check the file system even if it's marked as clean.

fsck -k This option will keep the existing bad blocks list.

fsck -l works "add to bad blocks list".  needs the filename. This adds the blocks listed in the specified file to the list of bad blocks

fsck -n [no] This option tells fsck to run in "no" mode, which means it will answer "no" to all questions and not make any changes to the file system.

fsck -p works "automatic" repair

fsck -r works

fsck -s works

fsck -t says option '-t' requires an argument

fsck -v works.  "verbose"

fsck -y works.  "yes"
