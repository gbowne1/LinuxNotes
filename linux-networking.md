# Linux Networking 101: A Beginner's Guide

Welcome to **Linux Networking 101** — a beginner-friendly guide that walks you through the basics of networking on Linux systems, especially using base distributions like **Debian**, **Ubuntu**, and other derivatives.

This guide is designed for beginners.

---

## Table of Contents

1. [What is Networking?](#what-is-networking)
2. [Basic Networking Terms](#basic-networking-terms)
3. [Physical Components](#physical-components)
4. [Understanding IP Addresses](#understanding-ip-addresses)
5. [Essential Network Commands](#essential-network-commands)
6. [Testing Your Network](#testing-your-network)
7. [Configuring Your Network](#configuring-your-network)
8. [Networking Protocols](#networking-protocols)
9. [Common Tools You Might Already Have](#common-tools-you-might-already-have)
10. [Further Learning](#further-learning)

---

## What is Networking?

Networking is how computers talk to each other. It can be through cables (wired) or through the air (wireless). At home, your devices connect to each other and to the internet using a router.

---

## Basic Networking Terms

- **Router** – Connects your home to the internet.
- **Switch** – Connects devices inside your home (like a wired hub).
- **Hub** – Older version of a switch, not smart.
- **NIC (Network Interface Card)** – Hardware in your computer that connects to the network.
- **Ethernet Cable** – A wire that connects devices to your router or switch.
- **Wi-Fi** – Wireless way of connecting to the internet.

---

## Physical Components

- **Modem** – Connects your home to your internet service provider (ISP).
- **Router** – Creates your home network.
- **Switch** – Expands the number of devices you can connect.
- **Cables (Cat5e/Cat6)** – Used to plug in devices.
- **Wireless Adapter** – Connects a device to Wi-Fi.

---

## Understanding IP Addresses

Each device on a network has an **IP address**. Think of it like a mailing address.

- IPv4 example: `192.168.1.10`
- IPv6 example: `fe80::1ff:fe23:4567:890a`

You can find your IP address with:

You can find your IP address with:

    ```bash
    ip a
    ```

or

    ```bash
    ifconfig
    ```

These commands show your network interfaces. Look for a section like `eth0` or `wlan0` (wired or wireless), and an `inet` line showing your IP address.

---

## Essential Network Commands

Here are some useful Linux network commands:

| Command       | What It Does                                        |
|---------------|-----------------------------------------------------|
| `ping`        | Check if another system is reachable                |
| `ping6`       | Same as `ping` but for IPv6                         |
| `ifconfig`    | View or configure network interfaces (deprecated)   |
| `ip a`        | View interface info (modern replacement for ifconfig) |
| `netstat`     | Show open ports and connections                     |
| `ss`          | Modern replacement for `netstat`                    |
| `traceroute`  | Show the path packets take to a host                |
| `mtr`         | Live traceroute with stats                          |
| `dig`         | Query DNS info                                      |
| `nslookup`    | DNS info (older tool, but still common)             |
| `host`        | Simple DNS lookup                                   |
| `arp`         | Show or modify the ARP cache                        |
| `scp`         | Copy files over SSH                                 |
| `rsync`       | Sync files locally or over SSH                      |
| `ssh`         | Secure remote login                                 |
| `ftp` / `sftp`| Transfer files over a network                       |
| `nmap`        | Scan local or remote networks                       |

---

## Testing Your Network

### Test Internet Connection

    ```bash
    ping 8.8.8.8
    ```

This checks if your system can reach Google's DNS server. You should see replies.

### Test DNS Resolution

    ```bash
    ping google.com
    ```

If `8.8.8.8` works but `google.com` does not, you likely have a DNS issue.

### Trace the Path to a Host

    ```bash
    traceroute google.com
    ```

Use `mtr` for a live version:

    ```bash
    mtr google.com
    ```

---

## Configuring Your Network

Use `nmtui` (text UI) on Debian-based systems:

    ```bash
    sudo nmtui
    ```

Bring interfaces up or down:

    ```bash
    sudo ifdown eth0
    sudo ifup eth0
    ```

Or using the `ip` command:

    ```bash
    sudo ip link set eth0 down
    sudo ip link set eth0 up
    ```

Request a new IP address (via DHCP):

    ```bash
    sudo dhclient
    ```

---

## Networking Protocols

| Protocol  | Description                                 |
|-----------|---------------------------------------------|
| TCP       | Reliable communication (web, email, etc.)   |
| UDP       | Fast, unreliable (video, games)             |
| ICMP      | Used by `ping` and `traceroute`             |
| DNS       | Resolves names to IP addresses              |
| DHCP      | Automatically gives devices IP addresses    |
| HTTP/S    | Used for web browsing                       |
| SSH       | Secure command-line access                  |
| FTP/SFTP  | File transfer protocols                     |

---

## Common Tools You Might Already Have

Linux systems often come with a wide set of networking tools. You may already have:

    bind, ip, netstat, ping, ping6, ifconfig, iptables, scp,
    nmap, traceroute, ansible, chef, ss, dig, nslookup, route,
    host, arp, iwconfig, hostname, mtr, whois, dhclient,
    ethtool, sshd, ssh-agent, ssh, rpcinfo, nmcli, nmtui,
    hostnamectl, ifdown, ifup, nc, socat, rsync, dnsmasq,
    telnet, ftp, sftp, netcat, lsof, fuser, sysctl, nsenter,
    getent, plog, modprobe, sar, ufw, iostat, vmstat, tc

Check if something is installed with:

    ```bash
    which nmap
    ```

If no result is returned, install it using:

    ```bash
    sudo apt install nmap
    ```

---

## Next Steps

In the next chapters, we'll look at:

- 🔐 Setting up SSH keys for passwordless login
- 🔥 Managing a firewall with `ufw`
- 📁 Sharing files between Linux and Windows
- 🌐 Running a local DNS with `dnsmasq`
- 📦 Automating setups with Ansible or Chef
- 📊 Monitoring traffic with tools like `iftop` and `vnstat`

---

## Learn More

- Use `man <command>` to learn about any tool
- Read `/etc/network/interfaces` (older systems)
- Or check `/etc/netplan/*.yaml` (newer Debian/Ubuntu)
- Visit: [https://linuxcommand.org](https://linuxcommand.org)

---

Happy Networking! 🛜🐧🚀

