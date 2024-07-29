# using the cat command

My cat is from cat (GNU coreutils) 8.30
My cat is in /usr/bin/cat

Theses are the only flags when used by themselves do not return `invalid option`

cat -b  Number all non-blank output lines, starting at 1. This is useful for identifying individual lines in a file, especially when dealing with large files or logs.

cat -e Display at the end of each line, and display a at the beginning of a line if it is empty. This makes it easier to see the boundaries of lines, especially in files where lines may wrap onto the next line due to terminal width limitations.

cat -n Number all output lines, starting at 1. This is similar to -b but includes blank lines as well.

cat -s Squeeze multiple adjacent empty lines, causing them to be replaced with a single empty line. This is useful for cleaning up files that contain excessive whitespace.

cat -t  Display tabs as ^I. This can help visualize tab characters, which are often invisible in many text editors and viewers.

cat -u Do not output the trailing newline character. This can be useful when you're processing files and don't want the extra newline at the end.

cat -v Display non-printing characters (except for LFD and TAB). This is useful for seeing hidden characters, such as spaces or tabs, that might not normally be visible.

cat -A Equivalent to -vAT. This displays non-printing characters, shows tabs as ^I, and displays a $ at the end of each line.

cat -E Equivalent to -vAE. This displays non-printing characters, shows tabs as ^I, and displays a $ at the end of each line, except for the last line.

cat -T Equivalent to -vAT. This displays non-printing characters, shows tabs as ^I, and displays a $ at the end of each line, except for the last line.
