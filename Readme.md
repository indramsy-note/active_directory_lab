# 01 Installing The Domain Controller

1. Use `sconfig` to:
    - Change the hostname
    - Change the IP address to static
    - Change the DNS Server to our own IP address

2. Install the Active Directory Windows Feature

```shell
Install-WindowsFeature AD-Domain-Services -IncludeManagementTools
```


```
Get-NetIPAddress
```

# 02 Joining the Workstation to the domain



```
Add-Computer -Domainname xyz -Credential xyz\Administrator -Force -Restart
```
