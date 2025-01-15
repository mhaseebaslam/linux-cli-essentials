# Networking Commands

## Network Interfaces and IP Addresses

- `ip addr show`: Displays network interfaces and their IP addresses. Useful for checking the status and configuration of network interfaces.
- `ip -s link`: Shows network statistics, including the number of packets transmitted and received, errors, and dropped packets.

## Sockets and Connectivity

- `ss -l`: Shows listening sockets. Useful for identifying which services are listening for incoming connections.
- `ping <host>`: Pings a host and outputs the results. Useful for checking the connectivity to a remote host.

## Netplan Configuration

- `cat /etc/netplan/*.yaml`: Displays the current Netplan configuration. Netplan is used for configuring network interfaces on Ubuntu.
- `sudo netplan try`: Tests a new configuration for a set period of time. If the configuration is not confirmed, it will revert to the previous configuration.
- `sudo netplan apply`: Applies the current Netplan configuration. This command is used to make changes to the network configuration take effect.

## Firewall Management

- `sudo ufw status`: Displays the status of the firewall. Useful for checking whether the firewall is active and which rules are in place.
- `sudo ufw enable`: Enables the firewall. This command activates the firewall to start filtering traffic.
- `sudo ufw disable`: Disables the firewall. This command deactivates the firewall, allowing all traffic through.
- `sudo ufw allow <port/service>`: Allows traffic on a specific port or service. Useful for opening ports for specific applications.
- `sudo ufw deny <port/service>`: Denies traffic on a specific port or service. Useful for blocking unwanted traffic.
- `sudo ufw delete allow/deny <port/service>`: Deletes an existing rule. Useful for removing previously set allow or deny rules.

## SSH and Remote Access

- `ssh <user@host>`: Connects to a remote host via SSH. Useful for securely accessing remote systems.
- `scp <source> <user@host>:<destination>`: Securely copies files between hosts. Useful for transferring files over an SSH connection.
