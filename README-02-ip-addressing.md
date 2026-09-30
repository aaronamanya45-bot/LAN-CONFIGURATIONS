# IP Addressing Commands

IP addressing is used to identify devices on a network.

## Windows

### View IP Address

```cmd
ipconfig
```

### View Detailed Information

```cmd
ipconfig /all
```

### Release IP Address

```cmd
ipconfig /release
```

### Renew IP Address

```cmd
ipconfig /renew
```

### Clear DNS Cache

```cmd
ipconfig /flushdns
```

## Linux

### Display IP Address

```bash
ip addr
```

or:

```bash
ip a
```

### Display Network Interfaces

```bash
ip link
```

### Display Routing Table

```bash
ip route
```

## Assign a Temporary IP Address

Linux:

```bash
sudo ip addr add 192.168.1.10/24 dev eth0
```

The parts mean:

* `sudo` = run with administrator privileges
* `ip addr add` = add an IP address
* `192.168.1.10` = IP address
* `/24` = subnet prefix
* `eth0` = network interface

## Remove an IP Address

```bash
sudo ip addr del 192.168.1.10/24 dev eth0
```

## Bring an Interface Up

```bash
sudo ip link set eth0 up
```

## Bring an Interface Down

```bash
sudo ip link set eth0 down
```

## Important

The interface name may not always be `eth0`.

You can check the actual interface name using:

```bash
ip link
```
