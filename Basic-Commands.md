## Networking 

```
ipconfig - Show information
```
```
netstat - show network traffic to host machine 
```
```
ping {IP} - send ping to another machine. External or internal
```


## Services 


## Accounts

```
net user - Shows all users
```
```
net user Username /add Password 
```
```
net user Username /add * (Hides the password being entered)
```
```
net localgroup {GroupName} /add  - add to a group ie administrators group
```
```
net user Username /delete - deletes the user account
```
```
wmic UserAccount where Name="user name" set PasswordExpires=False
```


## Shutdown Commands
```
shutdown  - will shut down the machine 
```
```
shutdown /r /t 100  - Reboot command after 100 seconds 
```
```
shutdown /m \\ MachineName /r /f - This will reboot a remote computer forcing all applications to close

```

## Windows System Info Commands
```
ver - Get the OS Version
```
```
sc query state=all - Show Services
```
```
tasklist /scvc - Show Services and processes
```
```
fsuntil fsinfo drives - List drives (Must be admin)
```
```
echo %USERNAME% - Current User 
```

## Windows Domain Commands 

```
net view /domain - Hosts in the current domain
```
```
net view /domain:{mydomain} - Hosts in {mydomain}
```
```
net user /domain - All users in the current domain
```
```
net localgroup Administrators  - List local Admins
```
```
net group "Domain Admins" /domain - List Users in Domain Admins
```
```
net group "Domain Controllers" /domain - List Domain Controllers in current Domain
```
```
net accounts /domain - Domain Password Policy
```
```
net share - Current SMB Shares
```
```
net sesssion | find / "\\" - Active SMB Shares
```
```
net share <share> c:\share - Share folder
```














