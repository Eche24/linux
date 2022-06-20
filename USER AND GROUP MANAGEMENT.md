#### Create , delete and modify local user account

`
useradd <username> 
`

`
useradd --shell /bin/othershell --home-dir /home/otherdirectory/<user>  
`

`passwd <username>
`

`
userdel <username>
`

`
userdel --remove <username> --- remove user and home directory
`

`
useradd --uid <uidnumber> <username> -- change uid number
`

`
useradd --system <system-name> -- add a system program 
`
#### modify user

`
usermod
`
