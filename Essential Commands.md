
## Create and manage hard links

Inode: keep track metadata, permission, last modify access time etc. the file link to inode. inode point to all data about a file.

`
$ stat <filename>  - to see the inode
`

## Hard links point to thesame inode of a file.

e.g sharing 5000 pics. huge space , used hard link to two users. after delete still have access to it.

`
$ ln <path_to_target_file> <path_to_link_file>
`
# limitations and considerations
only hardlink to files, not folders.
only hardlink to files on thesamce filesystem.


## Create and manage soft links (symbolic links)
softlinks: shortcuts of an file. like a path point a file.

`
$ ln -s <path_to_target_file>  <path_to_link_file>
`

`ls -l
 $ to see the softlink. but if the file is to long. used the 'readlink path_to_target_file'
`

# List, set and change file.

## Owners and Groups
Change group 'chgrp' command
`
chgrp <group-name> <filename>
`
list group

`
groups
`
change owner

`
chown <owner-name> <filename>
`
changing group and ownership together

`
chown <ownername>:<groupname> <filename>
`




## Octal Permissions
rwx
000 - 0
001 - 1
010 - 2
011 - 3
100 - 4
101 - 5
110 - 6
111 - 7









