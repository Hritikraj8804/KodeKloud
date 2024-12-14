## Commands Used

Here are some commonly used networking commands and their purposes:

### Basic Commands
- `ping <hostname/IP>`: Check the reachability of a host.
- `traceroute <hostname/IP>`: Display the route packets take to reach a host.
- `nslookup <domain>`: Query DNS for domain name or IP resolution.
- `dig <domain>`: Perform detailed DNS queries.

### Troubleshooting Commands
- `netstat -tuln`: Display active TCP/UDP ports and their statuses.
- `ss -tuln`: Display socket statistics (alternative to `netstat`).
- `tcpdump -i <interface>`: Capture network packets on a specified interface.
- `wireshark`: Graphical tool for detailed packet analysis.

### File Transfers and Requests
- `curl <url>`: Send HTTP requests from the command line.
- `wget <url>`: Download files from the web.
- `scp <source> <destination>`: Securely copy files between hosts.

### Advanced Commands
- `iptables -L`: List firewall rules.
- `ip addr`: Display IP addresses and network interfaces.
- `ifconfig`: Display or configure network interfaces (deprecated, use `ip` commands).
