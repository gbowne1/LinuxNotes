# using ps cmmand

ps -a
ps -c
ps -d
ps -e
ps -f
ps -g
ps -h
ps -j
ps -l
ps -m
ps -n
ps -o says format specification must follow -o
ps -p says list of process ID's must follow -p
ps -q says list of process ID's must follow -q
ps -r
ps -s
ps -t
ps -u sorts by user?
ps -v
ps -w
ps -x
ps -y says modifier -y without format -l makes no sense

ps -C says list of command names must follow -C
ps -F
ps -G says list of real groups must follow -G
ps -H
ps -L
ps -M sorts by label
ps -N sorts by PID
ps -O says format or sort specifications must follow -O
ps -P
ps -S
ps -T
ps -U says list of real users must follow -U
ps -V prints version ps from procps-ng 3.3.15
ps -X prints by PID then hex
ps -Z prints by label

## Some common uses of ps

    ps aux shows all processes running for all users
    ps -ef shows a full listing of all processes in a tree format
    ps -u username shows processes for a specific user
    ps aux --sort=-pcpu sorts processes by CPU usage (descending order)
    ps -o pid,user,command displays only the PID, user, and command for each process
