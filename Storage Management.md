
# Block Storage.

### Device Driver -  the kernel module used to access the physical device.
### Device File -    /dev/sda , having a file to represent the disk standard I/O can be used to read and write to disk. 

`
$ lscpu - list the cpu
$ lsmod - list module

`

## Loop Device.
Loop devices have files as the backend storage in place of physical storage.


### Using dd and Fallocate Command.

`
$ dd - disk duplicator
$ dd if=/dev/zero of=dd.disk bs=1M count=500 -  bs-block size, of- disk to write to, if- put zero, count- how much writing.

`

`
$ fallocate -l 500M fa.disk  - l - length
Fallocate -  quicker way of creating huge files because it allocates uninitialized blocks
`

# Partitioning Disk Device

### Common Patiotion table in Linux

MBR - Master Boot record, 2TB , Max partition is 4, and has it limitation.
GUID  - Globally Unique Identifer Disk, 8ZB. Max 128.

### Partitioning Tools

`
$ fdisk - interactive command
$ parted - partition Editor: support both MBR and  GPT. one-liner
$ gdisk -  GUID
$ cfdisk
`
### Creating a Partition Table.

`
$ fdisk /dev/sda

`

### FileSystem

#### creating an ext4 filesystem

`
$ mkfs.ext4 -L DATA /dev/<>
$ mkfs.xfs /dev/<>

`

### EFI system - booting filesystem

### Mounting filesystem: process of attaching a filesystem to a running system. 

#Swap Space

`
$ swapon --show
$ mkswap /dev/<> - used this partition as swap
$ swapon /dev/<> - used this partition 
$ swapoff /dev/<>

`
### Using a file as swap space

`
$ DD if=/dev/zero of=/swap bs=1M count=128 - using a input file in dev/zero(inifinite number of zero),
$ mkswap /swap

`



Logical Volume Manager
