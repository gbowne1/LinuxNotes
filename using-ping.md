# using the ping command

My ping is in /usr/bin/ping /usr/share/man/man8/ping.8.gz

My ping is `ping utility, iputils-s20180629`

## lowercase option flags

`ping -a` Audible ping. This makes ping produce a bell sound (ASCII 0x07) on each echo reply received.

`ping -b` Allow pinging a broadcast address.

`ping -c` says option requires an argument -- `c` and it is [count]: Stop after sending (and receiving) count ECHO_RESPONSE packets.

`ping -d`  Set the SO_DEBUG option on the socket being used.

`ping -f` Flood ping. Outputs packets as fast as they come back or one hundred times per second, whichever is more. Useful for testing network performance

`ping -h` Show help. Displays usage information and exits.

`ping -i` says option requires an argument -- `i` and is [interval]: Wait interval seconds between sending each packet. The default is to wait for one second between each packet.

`ping -l` says option requires an argument -- `l` [preload]: If preload is specified, ping sends that many packets as fast as possible before falling into its normal mode of behavior.

`ping -m` says option requires an argument -- `m`  [mark]: Tag the packets going out with the specified mark value.

`ping -n` Numeric output only. No attempt will be made to lookup symbolic names for host addresses

`ping -p` says option requires an argument -- `p` [pattern]: You may specify up to 16 "pad" bytes to fill out the packet you send. This is useful for diagnosing data-dependent problems in a network.

`ping -q` Quiet output. Nothing is displayed except the summary lines at startup time and when finished.

`ping -r` Bypass the normal routing tables and send directly to a host on an attached network.

`ping -s` option requires an argument -- `s` [packetsize]: Specifies the number of data bytes to be sent.

`ping -t` option requires an argument -- `t` [ttl]: Set the IP Time to Live.

`ping -v` prints the version same as -V and --version. may be also "verbose"

`ping -w` [deadline]: Specify a timeout, in seconds, before ping exits regardless of how many packets have been sent or received.

## uppercase option flags

`ping -A` Adaptive ping. Interpacket interval adapts to round-trip time, so that effectively not more than one (or more, if preload is set) unanswered probe is present in the network

`ping -B` Do not allow ping to change the source address of probes. The address is bound to one selected when ping starts.

`ping -D` Print timestamp (unix time + microseconds as in gettimeofday) before each line.

`ping -F` Flood ping (same as lowercase -f). Use with caution and only on internal networks.

`ping -I` [interface]: Set source address to specified interface address. This flag can be used if you have multiple interfaces and want to use a specific one for pinging.

`ping -L` Suppress loopback of multicast packets. This flag only applies if the ping destination is a multicast address.

`ping -M` [pmtudisc_opt]: Select Path MTU Discovery strategy. 'do' prohibits fragmentation, 'want' allows fragmentation at endpoints, 'dont' does not set DF flag.

`ping -N` Node info query/reply. Queries the node for its node info, and displays the results.

`ping -O` Report outstanding ICMP ECHO reply before sending next packet. This can be used to determine where packet loss is occurring.

`ping -Q` [tos]: Set Quality of Service-related bits in ICMP datagrams. tos can be decimal or hex number.

`ping -R` Record route. Includes the RECORD_ROUTE option in the ECHO_REQUEST packet and displays the route buffer on returned packets.

`ping -S` [sndbuf]: Set socket sndbuf. If not specified, it is selected to buffer not more than one packet.

`ping -T` [timestamp_option]: Set special IP timestamp options. timestamp_option can be 'tsonly' (timestamps only) or 'tsandaddr' (timestamps and addresses).

`ping -U` Print full user-to-user latency (the old behavior). Normally ping prints network round trip time, which can be different from user-to-user latency.

`ping -V` Version. Print version and exit (same as lowercase -v).

`ping -W` [timeout]: Time to wait for a response, in seconds. The option affects only timeout in absence of any responses, otherwise ping waits for two RTTs.

ping -V prints the version

## double dash flags

ping --version with command help