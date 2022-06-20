#### How to find the linux version and kernel release.
`sh
uname -a
`
#### Check a system current IP address.
`
ifconfig
ip addr show
`
#### Check for free disk space.
`
df -ah
`
#### How do you manage services on a system.
`
systemctl status <services>
`
#### Check the Size of a directory's contents on disks.
`
du -sh
`
#### Check or listen for open ports.
`
netstat -tulpn
`
#### Check CPU usage for a process

`
ps aux | grep <process name>
`
#### Check file that are open by a process
`
lsof -p <PID>
`
