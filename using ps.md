# using ps cmmand

The ps command is a fundamental tool in Unix-like operating systems for monitoring the status of processes.

`ps -a` Displays processes from all users except those of the current user.

`ps -c` Shows processes in a format that's suitable for use with awk.

`ps -d` Lists processes that have been detached from the terminal

`ps -e` quivalent to ps -E (deprecated), displays every process on the system.

`ps -f` Displays full-format listing. Shows the UID, PID, PPID, C, STIME, TTY, TIME, and CMD for each process.

`ps -g` Shows processes in a format that's suitable for use with getopts.

`ps -h` Human-readable format. Displays memory sizes in a human-readable format (e.g., KB, MB).

`ps -j` Displays processes in a job control format.

`ps -l` Long listing format. Shows the UID, PID, PPID, C, PRI, NI, ADDR, Z, STAT, TIME, and CMD for each process.

`ps -m` Displays processes in a format that's suitable for use with mail.

`ps -n`  Displays processes in a format that's suitable for use with news.

`ps -o` says format specification must follow -o and allows you to specify custom output columns.

`ps -p` says list of process ID's must follow -p and allows you to filter processes by PID.

`ps -q` says list of process ID's must follow -q and allows you to filter processes by name.

`ps -r` Reports processes in reverse order of termination.

`ps -s` Sorts processes by user ID.

`ps -t` Filters processes by terminal.

`ps -u` Sorts processes by user name.

`ps -v` Displays virtual memory usage.

`ps -w` Wide listing format. Shows the UID, PID, PPID, C, PRI, NI, ADDR, Z, STAT, TIME, and CMD for each process.

`ps -x` Displays processes that have no controlling terminal.

`ps -y` says modifier -y without format -l makes no sense. Displays processes in a format that's suitable for use with yppasswd.

## uppercase option flags

`ps -C` says list of command names must follow -C
`ps -F`
`ps -G` says list of real groups must follow -G
`ps -H`
`ps -L`
`ps -M` sorts by label
`ps -N` sorts by PID
`ps -O` says format or sort specifications must follow -O
`ps -P`
`ps -S`
`ps -T`
`ps -U` says list of real users must follow -U
`ps -V` prints version ps from procps-ng 3.3.15
`ps -X` prints by PID then hex
`ps -Z` prints by label

## Some common uses of ps

    ps aux shows all processes running for all users
    ps -ef shows a full listing of all processes in a tree format
    ps -u username shows processes for a specific user
    ps aux --sort=-pcpu sorts processes by CPU usage (descending order)
    ps -o pid,user,command displays only the PID, user, and command for each process
