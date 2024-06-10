# Using find

Here are the flags that can be used with and what they do

My version of `find` seems to be:

```shell
find (GNU findutils) 4.6.0.225-235f
```

My version of find comes from /usr/bin/find /usr/share/man/man1/find.1.gz /usr/share/info/find.info-2.gz
/usr/share/info/find.info-1.gz /usr/share/info/find.info.gz

## Lowercase flags

find -a says `find: invalid expression; you have used a binary operator '-a' with nothing before it.`

find -d says `find: warning: the -d option is deprecated; please use -depth instead, because the latter is a POSIX-compliant feature.`

find -o says `find: invalid expression; you have used a binary operator '-o' with nothing before it.`

## Uppercase flags

find -D says `find: Missing argument after the -D option.`

find -H lists files in the directory

find -L lists files in the directory. Tells
find to follow symbolic links and treat the file or directory pointed to by the symlink as the target of the search

find -O says `find: The -O option must be immediately followed by a decimal integer`. This instructs
find to descend into mounted filesystems during the search.

find -P lists files in the directory.  tells find to avoid following symbolic links altogether

Any flag not listed here did not return any results when used on the command line by itself
or reported invalid option.

there is a help at `find --help`

The usage is typically:
`find <starting_directory> <expression> <action>`

There is a manual here: <https://www.gnu.org/software/findutils/find>

By default,find starts from the current working directory.

you can also do:

`find -name` Example: `find /etc -name "hosts"`

`find -size` Example: `find . -size +10M`

`find -type` Example: `find /var -type f`

`find -print` Example: `find /home/user -name "*.txt" -print`

`find -delete` (use with caution) Example: `find /tmp -empty -delete`

`find -exec (executes a command)` Example: `find . -name "*.jpg" -exec convert {} -thumbnail 100x100 thumb_{}.jpg \;`

`find -depth` Example: `find /var -name "log" -depth`

`find -user` Example: `find /home -user root`

`find -group` Example: `find /tmp -group www-data`

`find -atime` Example: `find /var/log -atime +7`

`find -mtime` Example: `find /path/to/directory -mtime -3`

`find -empty` Example: `find /home -empty`
