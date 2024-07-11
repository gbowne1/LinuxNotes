# using nmap

Nmap 7.70 ( <https://nmap.org> )
Man page at (<https://nmap.org/book/man.html>)

nmap -a says option is ambiguous

nmap -b says "option requires an artument -- 'a`

nmap -d reporting?  [debug] used for printing debugging info

nmap -e says "option requires an argument -- 'e'. used to specify the external IP address to use when sending packets. This can be useful for bypassing IP restrictions or masquerading as a different host.

nmap -f requires root priv.  "fragscan". a type of stealthy SYN flood attack. Due to its potential misuse, it requires elevated permissions.

nmap -g says "option requires an argument -- 'g'. used to set the source port range for outgoing packets. This can be useful for avoiding detection or bypassing firewall rules.

nmap -h prints help.

nmap -i says "option requires an argument -- 'i'. used to specify the interface to use for outgoing packets. This can be useful when you want to send packets from a specific network interface.

nmap -l

nmap -m says "option requires an argument -- 'm'. used to select a script category or script ID to run against targets. This allows for highly targeted attacks or checks based on predefined scripts.

nmap -n Disables DNS resolution, causing Nmap to resolve hostnames to IP addresses only once. This can speed up scans significantly.

nmap -o says "option requires an argument -- 'o'.  used to specify the output file name for scan results. This allows you to save scan results to a file for later analysis.

nmap -p says "option requires an argument -- 'p`. used to specify ports to scan. You can specify single ports, ranges, or comma-separated lists.

nmap -q [quiet] Quiet mode. Reduces the amount of output Nmap produces, making it easier to parse scan results programmatically.

nmap -r Randomizes the sequence of hosts scanned. This can help avoid detection by firewalls or intrusion detection systems.

nmap -s says "option requires an argument -- 's`

nmap -t says option is ambiguous

nmap -u

nmap -v, can also use -vv and -vvv for different levels of verbosity.

nmap -w  [wait] used to specify the wait time between packets sent. This can be useful for controlling the rate of packet transmission.

## uppercase option flags

nmap -A Enables OS detection, version detection, script scanning, and traceroute. Essentially, it runs a full suite of tests to gather as much information as possible about the target.

nmap -D Used for specifying decoys to use in a scan. Decoys can help mask the real source of the scan traffic, making it harder to detect.

nmap -F Runs a fast scan, limiting the number of probes sent to each host. This reduces the time taken for the scan but might miss some services.

nmap -I Performs a ping scan using ICMP echo requests. This is a lightweight way to discover hosts on the network.

nmap -O Enables OS detection. Nmap tries to determine the operating system of the target host(s).

nmap -P Specifies the protocol to use for the scan. Common values include TCP (tcp), UDP (udp), and ICMP (icmp).

nmap -R Bypasses routers; i.e., it performs a direct connection scan. This is useful for discovering hosts on the local network segment.

nmap -S Specifies the scan type. Common values include SYN (syn), NULL (null), FIN (fin), Xmas (xmas), and others.

nmap -T Sets the timing template to use for the scan. Values range from Paranoid (slowest) to Insane (fastest).

nmap -V Prints the version of Nmap being used.

nmap --version
