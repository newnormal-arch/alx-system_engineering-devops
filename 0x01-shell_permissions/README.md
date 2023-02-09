Shell Permissions Commands

su betty : switches the current user to the user betty.
echo "$(id -u -n)" : prints the effective username of the current user.
echo "$(id -g -n)" : prints all the groups the current user is part of.
chown betty hello : changes the owner of the file hello to the user betty.
