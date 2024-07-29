# using scp

used to securely copy files and directories between two hosts
(local and remote, or between two remote hosts) over an encrypted SSH connection.

My scp is in /usr/bin/scp

typical usage is scp [options] source_file_path user@host:target_directory

`scp -c` Specifies the cipher to use for encryption. Useful for specifying stronger encryption methods if needed.

`scp -d` Enables debugging mode. Provides detailed information about the operations being performed.

`scp -f` Reads configuration data from a file instead of the default /etc/ssh/ssh_config.

`scp -i` Specifies the private key file to use for authentication.

`scp -l`  Specifies the user name to log in as.

`scp -o` Passes an option in SSH config file format to the ssh command.

`scp -p` Specifies the port number to connect to on the destination host.

`scp -q` Quiet mode. Causes scp to not print progress messages.

`scp -r`  Recursively copies entire directories.

`scp -t` Forces pseudo-terminal allocation. Can be useful for interactive sessions.

`scp -v` Verbose mode. Increases verbosity of messages displayed during operation.

`scp -B` Invokes program to execute locally after successful transfer.

`scp -C` Compresses the data during the transfer.

`scp -F` Specifies an alternative per-user configuration file.

`scp -P` Similar to -p, but specifies a path to a configuration file instead of a port number.

`scp -S` Specifies the path to a program to be executed locally after successfully transferring a file.

`scp -T` Disables pseudo-terminal allocation. Can speed up transfers of large amounts of data.

I couldn't find any version information on this
