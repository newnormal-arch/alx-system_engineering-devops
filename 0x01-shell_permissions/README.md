Shell Permissions Commands

su betty : switches the current user to the user betty.
echo "$(id -u -n)" : prints the effective username of the current user.
echo "$(id -g -n)" : prints all the groups the current user is part of.
chown betty hello : changes the owner of the file hello to the user betty.
touch hello : creates an empty file called hello.
chmod u+x hello : adds execute permission to the owner of the file hello.
chmod ug+x,o+r hello : adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.
chmod a+x hello : adds execution permission to the owner, the group owner and the other users, to the file hello.
chmod 007 hello : adds all permissions to the users only.
chmod 753 hello : adds a set of permissions to the file hello.
chmod --reference olleh hello : sets the mode of the file hello the same as olleh’s mode.
chmod a+X * : adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users.
mkdir -m 751 my_dir : creates a directory called my_dir with permissions 751 in the working directory.
chgrp school hello : changes the group owner to school for the file hello.
chown -R vincent:staff ./* : changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.
chown -h vincent:staff _hello : changes the owner and the group owner of _hello to vincent and staff respectively.
