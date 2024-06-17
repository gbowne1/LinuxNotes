# using mount

If I recall correctly only root can used most mount options so you have to be using root.

## lowercase option flags

`mount -a` says `mount: only root can use "--all" option`

`mount -c` says `mount: only root can use "--no-canonicalize" option`

`mount -f` says `mount: only root can use "--no-canonicalize" option`

`mount -h` prints help

`mount -i` prints system mounts

`mount -l` prints more system mounts

`mount -n` says `only root can use "--no-mtab" option`

`mount -o` says `mount: option requires an argument -- 'o'`

`mount -r` says `bad usage`. mounts the filesystem in read-only mode

`mount -s` prints even more mounts

`mount -t` says `mount: option requires an argument -- 't'`. This is used to mount a specific filesystem type. Usage: `mount -t [type] [device] [dir]`
and can also be used to list or show currently mounted filesystem types.

`mount -v` "verbose" prints even even more mounts in a verbose manner.

`mount -w` says `mount: only root can use "--read-write" option`

## uppercase option flags

`mount -B` says only root can use "--bind" option

`mount -F` says only root can use "--fork" option. Forks a new incarnation of mount for each device, used in combination with the -a option

`mount -L` says option requires an argument -- `L`. Mounts the partition with the specified label.

`mount -M` says only root can use "--move" option. Moves a subtree to a different location

`mount -N` says option requires an argument -- `N`

`mount -O` "options" says option requires an argument -- `O`.  Used in combination with the `-a`.  Uses the options field in /etc/fstab

`mount -R` says only root can use "--rbind" option. Remounts a subtree in a different location.

`mount -T` says option requires an agrument -- `T`. specifies a different /etc/fstab file

`mount -U` says option requires an argument -- `U`

`mount -V` reports version from util-linux 2.33.1 (libmount 2.33.1)

## double -- option flags

--fork
--bind
--move
--rbind
--all
--no-canonicalize
--no-mtab
