# using umount

umount is an unmount command for unmounting devices.
my umount is from umount from util-linux 2.33.1 (libmount 2.33.1: selinux, smack, btrfs, namespaces, assert, debug)
its in umount: /usr/bin/umount /usr/sbin/umount.udisks2 /usr/sbin/umount.nfs4 /usr/sbin/umount.nfs /usr/share/man/man2/umount.2.gz /usr/share/man/man8/umount.8.gz

Unsure if most/all umount commands must be done as root and require su/sudo or root priv.

`umount -a` --all says only root can use `--all` option
`umount -c` only root can use --no-canonicalize option
`umount -d` says bad usage
`umount -f` only root can use --force option
`umount -h` help
`umount -i` says bad usage
`umount -u` says bad usage
`umount -l` says bad usaage
`umount -n` says only root can use --no-mtab option
`umount -q` says bad usage
`umount -r` says only root can use --read-only opton
`umount -t` says option requires an arugment -- `t` 

## uppercase option flags

`umount -A` says only root can use `--all-targets` option
`umount -N` says option requires an argument -- `N`
`umount -O` says option requires an argument -- `O`
`umount -R` says option requires an argument -- `R`
`umount -V` prints the version

man pages are at `man umount`

