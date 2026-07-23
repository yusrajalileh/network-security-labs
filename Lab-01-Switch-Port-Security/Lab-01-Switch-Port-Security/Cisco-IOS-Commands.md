# Cisco IOS Commands

## Configure Port Security
```bash
enable

configure terminal
interface range fa0/1-2
switchport mode access
switchport port-security
switchport port-security maximum 1
switchport port-security mac-address sticky
switchport port-security violation restrict
```

## Disable Unused Ports
```bash
interface range fa0/3-24
shutdown
```

## Verification Commands
```bash
show port-security
show port-security interface fa0/1
show port-security address
show running-config
```
