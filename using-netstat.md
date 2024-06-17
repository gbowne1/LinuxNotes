# using netstat

My netstat is /usr/bin/netstat /usr/share/man/man8/netstat.8.gz
My version is net-tools 2.10-alpha

## lowercase flags

netstat -a  displays information about all network connections, including active, listening, and inactive connections (sockets) on your system

netstat -c  provides statistics about network activity, but actual implementation might be system dependant

netstat -d  information about the kernel's network connections and routing tables, but output might vary slightly depending on your system and kernel version

netstat -e  information about all network interfaces, including active connections, routing tables, and interface statistics

netstat -f  says `netstat: feature AF BLUETOOTH' not supported. Please recompile 'net-tools' with newer kernel source or full configuration.`

netstat -g  shows group memberships as a table

netstat -i  shows the kernel interface table

netstat -l

netstat -n displays information about network connections on your system, with a key characteristic; it shows IP addresses instead of hostnames

netstat -o displays information about network connections, but with a focus on kernel-level details related to the connections

netstat -p shows items by process? displays information about network connections, along with the process ID (PID) and name of the program that owns each connection

netstat -r shows the kernel ip routing table.  displays the kernel's routing table

netstat -s "summary" shows provides summary statistics about various aspects of network activity

netstat -t shows tcp/ip information. Usage depends on your specific system and kernel version. Somewhat similar to `-a`

netstat -u displays information about network connections that use UDP (User Datagram Protocol

netstat -v "verbose" offers a very detailed view of network connections on your system

netstat -w output depends on system and kernel version(s). Might display warnings.  Might display listening TCP socket's.

netstat -x displays information about network connections involving Unix domain sockets.

## uppercase flags

netstat -A requires an argument. displays information about network connections involving Unix domain sockets.

netstat -C same as -c

netstat -F displays information about network connections, with focus on FQDN's (Fully Qualified Domain Names)

netstat -M says no support for `ip_masquerade` on this system. usage would depend on system and kernel implementation.

netstat -N displays information about network connections while avoiding DNS resolution

netstat -S says no support for `AF INET (sctp) on this system.

netstat -U Might not actually exist, but could be `-u`.

netstat -V reports the version number

netstat -W might be the same as `-w`

netstat -Z says`SELinux is not enabled on this machine.`
