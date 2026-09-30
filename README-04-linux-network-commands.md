# Linux Network Configuration Commands

Linux provides many commands for configuring and troubleshooting networks.

## 1. Display IP Addresses

```bash
ip addr
```

Short form:

```bash
ip a
```

## 2. Display Interfaces

```bash
ip link
```

## 3. Display Routing Table

```bash
ip route
```

## 4. Test Connectivity

```bash
ping 8.8.8.8
```

## 5. Test DNS

```bash
nslookup google.com
```

or:

```bash
dig google.com
```

## 6. Trace a Route

```bash
traceroute google.com
```

## 7. Add an IP Address

```bash
sudo ip addr add 192.168.1.20/24 dev eth0
```

## 8. Remove an IP Address

```bash
sudo ip addr del 192.168.1.20/24 dev eth0
```

## 9. Enable an Interface

```bash
sudo ip link set eth0 up
```

## 10. Disable an Interface

```bash
sudo ip link set eth0 down
```

## 11. Add a Default Gateway

```bash
sudo ip route add default via 192.168.1.1
```

## 12. Display Open Ports

```bash
ss -tuln
```

## 13. Display Network Statistics

```bash
ip -s link
```

## 14. Show DNS Configuration

```bash
resolvectl status
```

## 15. NetworkManager

On systems using NetworkManager:

```bash
nmcli device status
```

Display connections:

```bash
nmcli connection show
```

## Note

Modern Linux systems normally use the `ip` command instead of the older `ifconfig` command.
