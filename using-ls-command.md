# Using the ls command in linux

Using the ls command Anything not in this list doesn't return anything.  My ls comes from `ls (GNU coreutils) 8.30`, and installed to `/usr/bin/ls`

## Flags

### Lowerrcase flags

`ls -a` directory listing in two columns. this only includes dotfiles. used to list all files and directories in the current directory, including hidden ones

`ls -b` Might not actually exist, although it returns a listing. Might not be a standard option flag

`ls -c` sorts the directory listing by modification time, with the most recently modified files appearing at the bottom by default

`ls -d` lists only . directories. used to list only the directories within the current directory, excluding regular files and other entries

`ls -f` This shows dotfiles that start with `.` and provides a more informative listing of files in your directory by adding suffix characters to filenames to indicate their type.

`ls -g` This shows permissions and displays information about the group ownership of files and directories in the current directory

`ls -h` displays file sizes in a human-readable format,

`ls -i` displays the inode number for each file and directory in the current directory listing

`ls -k` displays file sizes in kilobytes (KB), making it a specific way to show human-readable sizes. `ls -h` might be a better choice.

`ls -l` This shows permissions. provides a detailed listing format for files and directories in the current directory.

`ls -m` directory listing, comma separated. might not be a standard option.

`ls -n` This shows permissions. displays user and group IDs (numeric identifiers) instead of usernames and group names in the output

`ls -o` This shows permissions. might not be a standard option.

`ls -p` displays the process ID (PID) associated with each directory in the listing, if the directory is currently being accessed by another process

`ls -q` "quiet". offers a silent mode, suppressing the usual output of filenames and suppressing any error messages. good for script usage.

`ls -r` This is a backwards reverse directory listing. displays the contents of directories in a reverse order, starting from the last entry (lexicographically) to the first.

`ls -s` This shows files with their sizes. displays the total size occupied by all files in the current directory, in blocks.

`ls -t` sorts the directory listing by modification time, displaying the files that were last modified first

`ls -u` displays the file listing sorted by the last access time of the files

`ls -v` "verbose" displays the verbose output of the ls command

`ls -w` requires some sort of argument to work.  not a standard option flag.

`ls -x` not a standard option flag.

### Uppercase flags

`ls -A`

`ls -B`

`ls -C`

`ls -D`

`ls -F`  ends each entry with / in a wide format

`ls -G`

`ls -H`

`ls -I` requires an argument

`ls -L`

`ls -N`

`ls -Q` all entries appear in between double quotes in a wide format

`ls -R` very interesting output when done by itself

`ls -S`

`ls -T` requires an argument.

`ls -U`

`ls -X` lists dirs/folders on the left half of a wide format output

`ls -Z` lists all entries with a ? in a wide format
