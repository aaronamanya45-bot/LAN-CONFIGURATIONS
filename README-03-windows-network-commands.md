# WINDOWS NETWORK CONFIGURATION COMMANDS

These commands are commonly used in Windows Command Prompt.

## 1. Display IP Information

```cmd
ipconfig
```

Detailed information:

```cmd
ipconfig /all
```

## 2. Release an IP Address

```cmd
ipconfig /release
```

## 3. Renew an IP Address

```cmd
ipconfig /renew
```

## 4. Clear DNS Cache

```cmd
ipconfig /flushdns
```

## 5. Test Connectivity

```cmd
ping 192.168.1.1
```

## 6. Trace a Route

```cmd
tracert google.com
```

## 7. Test DNS

```cmd
nslookup google.com
```

## 8. View ARP Table

```cmd
arp -a
```

## 9. View Routing Table

```cmd
route print
```

## 10. View Network Connections

```cmd
netstat -ano
```

The `-o` option displays the process ID associated with connections.

## 11. View Network Configuration

```cmd
netsh interface ip show config
```

## 12. Reset TCP/IP

```cmd
netsh int ip reset
```

## 13. Reset Winsock

```cmd
netsh winsock reset
```

After some reset commands, Windows may require a restart.

## 14. Display Network Interfaces

```cmd
netsh interface show interface
```

## 15. Test a Specific Port

PowerShell:

```powershell
Test-NetConnection google.com -Port 443
```

## COMMAND WINDOWS TROUBLESHOOTING ORDER

```text
ipconfig
     ↓
ping 127.0.0.1
     ↓
ping local gateway
     ↓
ping 8.8.8.8
     ↓
nslookup google.com
     ↓
tracert google.com
```
