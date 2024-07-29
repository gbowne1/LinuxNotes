# using tar

My tar is tar (GNU tar) 1.30

it is in /usr/bin/tar /usr/include/tar.h /usr/share/man/man1/tar.1.gz /usr/share/man/man3/tar.3tcl.gz

## lowecase flags

`tar -b` Block size. Specifies the block size to be used for tape archives. This is typically used when working with tape drives.
`tar -c` says coward if used by itself. Create. Creates a new archive. You need to specify the name of the archive after this flag.
`tar -d` Diff. Shows differences between an archive file and the files it contains.
`tar -f` File. Allows you to specify the name of the archive file.
`tar -g` GNU format. Uses the GNU tar format, which allows for better handling of sparse files and extended attributes.
`tar -r` Append. Adds files to an existing archive.
`tar -s` List. Lists the contents of an archive.
`tar -t` Table. Lists the table of contents of an archive.
`tar -u` Update. Updates an existing archive by adding files not already present.
`tar -x` Extract. Extracts files from an archive.

## uppercase flags

`tar -A` Add-File. Adds one or more files to an existing archive.
`tar -C` Change Directory. Changes to a directory before performing any operations.
`tar -F` File. Similar to -f, but requires the archive name to follow immediately.
`tar -H` Follow Symlinks. Follow symbolic links in the operation being performed.
`tar -I` Include. Includes files matching a pattern in the operation.
`tar -K` Kibibytes. Sets the block size in kibibytes.
`tar -L` Follow Links. Follows links in the operation being performed.
`tar -N` Newer. Only adds newer files to the archive.
`tar -T` Tape. Reads names from a file.
`tar -V` Verbosely. Verbose output.
`tar -W` Warning. Warnings instead of errors.
`tar -X` Exclude. Excludes files matching a pattern from the operation.

## double dash flags

--delete Deletes files from an archive.
--help Displays help text.
--usage Displays usage information.
--test-label sts whether an archive label matches a given string.
--same-order Preserves order of files in the archive.
--verify Verifies the integrity of an archive.
--version Displays version information.