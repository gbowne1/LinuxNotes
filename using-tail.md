# using tail

My tail is from tail (GNU coreutils) 8.30.
it is in /usr/bin/tail

`tail -b` which displays the last part of files.  `tail -b <number_of_bytes> filename`

`tail -c` requires an argument. display the last part of files based on the number of characters (bytes) from the end of the file
`tail -c <number_of_characters> filename`

`tail -f` this option is "follow". `tail -f filename`

`tail -l`

`tail -n` allows you to specify the number of lines from the end of a file to display. `tail -n 1 filename`

`tail -q` used to suppress the header line that normally precedes the output.

`tail -s` used to delay the start of the output.  `tail -s seconds -f filename`

`tail -v` says `==> standard input <==`.  Tail attempting to read from standard input? verbose?

`tail -z` sed to treat empty lines as delimiters between records. `tail -z filename`

`tail -F` used to treat empty lines as delimiters between records.

## other flags

`tail --version`

`tail --help`
