# using iptables

only preliminary option flag testing has been done here.

## lowercase option flags

`iptables -b` says Unknown arg "null"

`iptables -c` says option "-c" requires an argument. Chain. Specifies the chain to which the rule will be appended. This is mandatory because every rule must belong to a chain.

`iptables -d` says option "-d" requires an argument. Destination. Matches packets whose destination address matches the specified address. Requires an argument specifying the destination address.

`iptables -f` says no command specified. Fragment. Matches fragments of fragmented packets. This option is used internally by iptables and does not accept an argument.

`iptables -g` says option "-g" requres an argument. Generic. Used internally by iptables for generic processing and does not accept an argument.

`iptables -h` prints the help

`iptables -i` says option "-i" requres an argument. In. Specifies the network interface(s) via which a packet is coming. Requires an argument specifying the interface name.

`iptables -j` says option "-j" requres an argument. Jump. Specifies the target of the rule; i.e., what to do with the packet that matches this rule. Requires an argument specifying the target.

`iptables -m` says option "-m" requres an argument. Match. Specifies the match to use. This is used to classify the packet against a set of criteria. Requires an argument specifying the match to use.

`iptables -n` says no command specified. Numeric. Do not resolve service names. This speeds up loading of rules by avoiding DNS lookups.

`iptables -o` says option "-o" requres an argument. Output. Specifies the network interface(s) via which a packet is going. Requires an argument specifying the interface name.

`iptables -p` says option "-p" requres an argument. Protocol. Specifies the protocol of the rule. Requires an argument specifying the protocol (e.g., tcp, udp).

`iptables -s` says option "-s" requres an argument. Source. Matches packets whose source address matches the specified address. Requires an argument specifying the source address.

`iptables -t` says option "-t" requres an argument. Table. Specifies the table to which the rule belongs. Requires an argument specifying the table name.

`iptables -v` says no command specified. Verbose. Provides verbose output, showing details of the rule processing.

`iptables -w` says no command specified. Wait. Causes iptables to pause for a user-specified time period, waiting for packets to pass through the filter. Requires an argument specifying the wait time in seconds.

## uppercase option flags

`iptables -A` says option "-A" requres an argument

`iptables -C` says option "-C" requres an argument

`iptables -D` says option "-D" requres an argument

`iptables -E` says option "-E" requres an argument

`iptables -F` says permission denied, you must be root

`iptables -I` says option "-I" requres an argument

`iptables -L` says permission denied, you must be root

`iptables -M` says option "-M" requres an argument

`iptables -N` says option "-N" requres an argument

`iptables -P` says option "-P" requres an argument

`iptables -R` says option "-R" requres an argument

`iptables -S` says No chain/target/match by that name

`iptables -V` returns the version information

`iptables -W` says wait value required

`iptables -X` says permission denied, you must be root

`iptables -Z` says permission denied, you must be root
