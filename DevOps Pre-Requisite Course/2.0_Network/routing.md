# Networking Commands: ip link, ip route, route, ip addr, ip route add, ip addr add

This document provides a concise guide to essential networking commands for managing and configuring network interfaces, routes, and IP addresses in Linux environments.

## 1. `ip link`
The `ip link` command is used to display or modify network interfaces.

### Usage Examples
- **Display all network interfaces:**
  ```bash
  ip link show
  ```
- **Bring an interface up:**
  ```bash
  ip link set <interface> up
  ```
- **Bring an interface down:**
  ```bash
  ip link set <interface> down
  ```
- **Change the MTU of an interface:**
  ```bash
  ip link set <interface> mtu <value>
  ```

---

## 2. `ip route`
The `ip route` command is used to display and manipulate the kernel routing table.

### Usage Examples
- **Display the routing table:**
  ```bash
  ip route show
  ```
- **Delete a route:**
  ```bash
  ip route del <destination-network> via <gateway-ip> dev <interface>
  ```

---

## 3. `route`
The `route` command is an older tool for managing the routing table. It has largely been replaced by `ip route` but is still available in some systems.

### Usage Examples
- **Display the routing table:**
  ```bash
  route -n
  ```
- **Add a route:**
  ```bash
  route add -net <network> netmask <subnet-mask> gw <gateway-ip> dev <interface>
  ```
- **Delete a route:**
  ```bash
  route del -net <network> netmask <subnet-mask> gw <gateway-ip> dev <interface>
  ```

---

## 4. `ip addr`
The `ip addr` command is used to display or modify IP addresses assigned to network interfaces.

### Usage Examples
- **Display IP addresses of all interfaces:**
  ```bash
  ip addr show
  ```
- **Display IP addresses for a specific interface:**
  ```bash
  ip addr show dev <interface>
  ```

---

## 5. `ip route add`
The `ip route add` command is used to add a static route to the kernel routing table.

### Usage Examples
- **Add a static route to a network:**
  ```bash
  ip route add <destination-network> via <gateway-ip> dev <interface>
  ```
  Example:
  ```bash
  ip route add 192.168.1.0/24 via 192.168.0.1 dev eth0
  ```

---

## 6. `ip addr add`
The `ip addr add` command is used to assign an IP address to a network interface.

### Usage Examples
- **Add an IP address to an interface:**
  ```bash
  ip addr add <ip-address>/<subnet-mask> dev <interface>
  ```
  Example:
  ```bash
  ip addr add 192.168.1.10/24 dev eth0
  ```

---

### Notes
- The `ip` command suite is part of the `iproute2` package, which provides modern tools for network management.
- The `route` command is considered deprecated in many distributions and is replaced by `ip route`.

### Related Commands
- `ifconfig`: A legacy command for network interface configuration.
- `netstat`: A legacy tool for displaying network connections, routing tables, and interface statistics.
- `ss`: A modern replacement for `netstat`.

### Conclusion
These commands provide powerful utilities for network configuration and management. DevOps engineers and system administrators should familiarize themselves with the `ip` suite as it offers advanced features and is widely supported.
