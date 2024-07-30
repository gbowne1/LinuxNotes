# Using the ls command in linux

Using the ls command Anything not in this list doesn't return anything.  My ls comes from `ls (GNU coreutils) 8.30`, and installed to `/usr/bin/ls`

## Flags

### Lowercase flags

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

`ls -A` shows all files and directories except those whose names begin with a dot (.).

`ls -B`  This flag uses a block size of one kilobyte for displaying file sizes.

`ls -C`  This flag aligns the output in columns

`ls -D`  This flag prints the parent directory name in the last column of the output

`ls -F`  Ends each entry with a character indicating the type of file

`ls -G` Similar to -F, but uses a different set of symbols. It's another way to visually distinguish file types in the output.

`ls -H`  Like -F, but treats symlinks specially, showing the target of the link instead of the symlink itself.

`ls -I` requires an argument. `ls -I <pattern>` Shows all files and directories except those matching the given pattern. You need to replace <pattern> with the actual pattern you want to exclude.

`ls -L` When used with symbolic links, this flag shows the contents of the linked-to directory instead of the link itself.

`ls -N` Appends a trailing slash (/) to directories. This makes it easier to distinguish them from regular files in the output.

`ls -Q` all entries appear in between double quotes in a wide format. Encloses filenames in double quotes. This is especially useful when dealing with filenames that contain spaces or special characters.

`ls -R` Recursively lists subdirectories. If used alone, it will recursively list all subdirectories starting from the current directory.

`ls -S` Sorts files by size, largest first. This is useful for quickly finding the largest files in a directory.

`ls -T` requires an argument.  Adds a time stamp to each file. The timestamp indicates the last modification time of the file.

`ls -U` Uses a less ambiguous format for timestamps. Instead of the standard MMM DD HH:MM:SS YYYY, it uses YYYY-MM-DD HH:MM.

`ls -X` lists dirs/folders on the left half of a wide format output. Lists directories on the left half of the screen when using a wide format. This helps in scanning through directories quickly.

`ls -Z` lists all entries with a ? in a wide format. Displays a question mark (?) at the end of each filename. This is part of the "wide" format, similar to -F and -G.

`ls -lCF --color=auto` This command lists files in long format (-l), adds slashes at the end of directories (-C), and colors the output (--color=auto).
