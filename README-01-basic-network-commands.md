# Basic Network Commands

These are some of the basic commands used to view network information and test network connectivity.

## 1. `hostname`

Displays the name of the computer.

```bash
hostname
```

Example:

```text
DESKTOP-123ABC
```

## 2. `ping`

Tests whether another device can be reached across a network.

```bash
ping 8.8.8.8
```

You can also ping a website:

```bash
ping google.com
```

## 3. `ipconfig`

Used mainly on Windows to display IP configuration.

```cmd
ipconfig
```

To display more detailed information:

```cmd
ipconfig /all
```

## 4. `ipconfig /release`

Releases the current DHCP IP address.

```cmd
ipconfig /release
```

## 5. `ipconfig /renew`

Requests a new IP address from the DHCP server.

```cmd
ipconfig /renew
```

## 6. `ipconfig /flushdns`

Clears the DNS cache.

```cmd
ipconfig /flushdns
```

## 7. `arp`

Displays the ARP table.

```cmd
arp -a
```

## 8. `route`

Displays the routing table.

```cmd
route print
```

## 9. `netstat`

Displays active network connections.

```cmd
netstat
```

To display listening ports:

```cmd
netstat -an
```

## 10. `nslookup`

Checks DNS information.

```cmd
nslookup google.com
```

## 11. `tracert`

Shows the path packets take to a destination on Windows.

```cmd
tracert google.com
```

## 12. `pathping`

Combines features of `ping` and `tracert`.

```cmd
pathping google.com
```

## Summary

These commands are useful when checking whether a computer is connected to a network and when troubleshooting basic network problems.
