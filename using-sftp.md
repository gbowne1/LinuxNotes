# using sftp

To install
`sudo apt update`
`sudo apt install openssh-server`

## configure

`sudo nano /etc/ssh/sshd_config` (or use whatever editor you like)

At this point, I think it would be a great idea to create a chroot jail.

This would primarily be to restrict SFTP users to their home directory, you can create a chroot jail.

Add the following to your `/etc/ssh/sshd_config`

Match Group sftp
    ChrootDirectory /var/sftp/%u
    ForceCommand internal-sftp
    AllowTcpForwarding no
    X11Forwarding no

You might also add Subsystem sftp internal-sftp to this.

Then create an sftp group:

`sudo groupadd sftp`

Add users to the sftp group:

`sudo usermod -aG sftp username`

Set up proper directory structure:

`sudo mkdir /var/sftp/username/uploads`
`sudo chown username:sftp /var/sftp/username/uploads`
`sudo chmod 755 /var/sftp/username/uploads`

## firewall

If you're using UFW (Uncomplicated Firewall), allow SSH/SFTP:

`sudo ufw allow ssh`

Use key-based authentication:
For better security, consider using SSH keys instead of passwords:

`ssh-keygen -t rsa -b 4096`
ssh-copy-id username@your_server_ip

Disable password authentication (optional):
In /etc/ssh/sshd_config, set:

PasswordAuthentication no

Limit user access:
You can limit which users can use SFTP by adding to /etc/ssh/sshd_config:

AllowUsers user1 user2

Log SFTP activities:
Add to /etc/ssh/sshd_config:

Subsystem sftp /usr/lib/openssh/sftp-server -f AUTH -l INFO

Consider rate limiting:

To prevent brute force attacks, you might want to install and configure fail2ban.

# setup access

Enable SFTP Subsystem: Ensure that the SFTP subsystem is enabled by looking for the line that says Subsystem sftp /usr/lib/openssh/sftp-server.

If it's commented out (starts with a #), remove the # to uncomment it. save the changes and restart the service

`sudo systemctl restart ssh`

By default, users will not have a home directory under /var/sftp, so you'll need to create one for them.

This is a common practice to separate SFTP traffic from regular FTP traffic

`sudo mkdir /var/sftp/username`

Set the permissions so that the owner has read, write, and execute permissions, and others have no permissions.

`sudo chown root:root /var/sftp/username`

`sudo chmod 755 /var/sftp/username` one could also use 700 though

Edit the user's shell to use SFTP instead of the default shell. This can be done by adding the following line to the end of the /etc/passwd file for the user:

`username:x:1001:1001::/var/sftp/username:/usr/lib/openssh/sftp-server`

Re restart the service yet again

`sudo systemctl restart ssh`

sftp username@server_ip

make sure the permissions are good with `ls -la`
