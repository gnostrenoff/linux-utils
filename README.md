# linux-utils

This repository contains some useful linux command

## __SSH__
### ssh config
-> Simplify remote access command
create a ***config*** file in your ~/.ssh folder.
Each host you want to reach are configured in this ***config*** file. Here is an example of template for one host:
```bash
Host <hostNickName>
HostName <hostfullName>
IdentityFile ~/.ssh/certif.pem
User <theUser>
```

## __Git__
[Here](http://ndpsoftware.com/git-cheatsheet.html#loc=stash;) is a link heading to a nice interactive cheatsheet.

## __Docker__
Coming ...

## __Utils__
#### __Kill process by name__
```bash
pkill -f <processName>
```
#### __Get your machine's core number__
```bash
cat /proc/cpuinfo | grep processor | wc -l
```
#### __Disable service autostart__
```bash
update-rc.d <service-name> disable
```
