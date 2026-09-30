# Cisco Router and Switch Commands

These commands are commonly used when configuring Cisco routers and switches.

## 1. Enter Privileged EXEC Mode

```text
enable
```

## 2. Enter Global Configuration Mode

```text
configure terminal
```

Short form:

```text
conf t
```

## 3. Set Device Name

```text
hostname R1
```

Example:

```text
hostname Router1
```

## 4. Configure an Interface

```text
interface gigabitEthernet 0/0
```

## 5. Assign an IP Address

```text
ip address 192.168.1.1 255.255.255.0
```

## 6. Enable the Interface

```text
no shutdown
```

## 7. Disable an Interface

```text
shutdown
```

## 8. Exit Configuration Mode

```text
exit
```

## 9. Return to Privileged Mode

```text
end
```

## 10. Display Interfaces

```text
show ip interface brief
```

## 11. Display Running Configuration

```text
show running-config
```

## 12. Display Startup Configuration

```text
show startup-config
```

## 13. Display IP Routing Table

```text
show ip route
```

## 14. Test Connectivity

```text
ping 192.168.1.2
```

## 15. Save Configuration

```text
copy running-config startup-config
```

Short form:

```text
write memory
```

## 16. Display VLANs

```text
show vlan brief
```

## 17. Display CDP Neighbors

```text
show cdp neighbors
```

## 18. Display MAC Address Table

```text
show mac address-table
```

## Basic Router Configuration Example

```text
enable
configure terminal

hostname R1

interface gigabitEthernet 0/0
ip address 192.168.1.1 255.255.255.0
no shutdown

end

copy running-config startup-config
```

## Important

Cisco commands depend on the device model and IOS version.
