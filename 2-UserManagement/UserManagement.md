## User Management in Linux

- User management in Linux involves creating, modifying, and deleting user accounts, setting permissions, managing groups, and configuring authentication.

## Key Files
* /etc/passwd – Stores user account details.
* /etc/shadow – Stores encrypted user passwords.
* /etc/group – Stores group information.
* /etc/gshadow – Stores secure group details.

## Creating Users
- Create a User
 `sudo adduser username`
Automatically creates the home directory /home/username.

     Alternative

     `sudo useradd  username`  will not create Home directory. (user -m to create with a home directory)      `sudo useradd  -m username`

## Managing Password

- Set User Password  `sudo passwd username`
-  Password Expiry `chage -M 90 username`
- Lock User `passwd -l username`
- Unlock User `passwd -u username`

## Modifying Users

- Change the username `usermod -l new_username old_username`
- Change the home directory `usermod -d /new/home/directory -m username`

## Deleting Users
 - To remove a user but keep their home directory `userdel username`
 - To remove a user and their home directory `userdel -r username`

## Working with Groups

- Creating Groups `groupadd groupname`
- Adding Users to Groups `usermod -aG groupname username`
- Remove User from Group `gpasswd -d username groupname`
- Viewing Group Memberships `groups username`

## Switch User
`su - username`

