# __linux-utils__

This repository contains some useful linux commands.

## __SSH__
#### Generate key pair
```bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```
#### ssh config
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
#### Cheatsheet
[Here](http://ndpsoftware.com/git-cheatsheet.html#loc=stash;) is a link heading to a nice interactive cheatsheet.
#### Pretty tree
```bash
git log --graph --oneline --all --decorate=short
```

## __Docker__
#### Cheatsheet
[here](https://github.com/wsargent/docker-cheat-sheet) is a link heading to a nice cheatsheet.
#### Utils


## __Utils__
#### __Change user name__
Add a temporary user
```bash
sudo adduser temporary
```
Add this user to sudoers
```bash
sudo adduser temporary sudo
```
Then log out, and log in using created user.
```bash
sudo usermod -l newUsername oldUsername
usermod -d /home/newHomeDir -m newUsername
```
( You may need to killall oldUsername before executing the 2 commands above to make sure no process is running for this user)
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
#### __Get public ip__
```bash
wget http://ipinfo.io/ip -qO -
```
