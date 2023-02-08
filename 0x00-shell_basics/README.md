ALX Systems Engineering Commands

pwd : prints the absolute path name of the current working directory.
ls : displays the contents list of your current working directory.
cd : changes the working directory to the user's home directory.
ls -l : lists the contents of the current working directory in long format.
ls -la : lists the contents including hidden files in long format.
ls -lna : lists content including hidden files, user and group IDs displayed numerically.
mkdir /tmp/my_first_directory : creates a new empty directory call my_first_directory inside the tmp directory.
mv /tmp/betty /tmp/my_first_directory/ : moves the file betty from the tmp directory into the my_first_directory directory.
rm /tmp/my_first_directory/betty : deletes or removes the file called betty inside the my_first_directory directory.
rmdir /tmp/my_first_directory/ : deletes or removes the empty directory called my_first_directory.
cd - : changes the working directory to the previous one.
ls -al . .. /boot : lists all files in the directory and the parent of the working directory and the /boot directory, in long format.
file /tmp/iamafile : prints the type of file named iamafile
ln -s /bin/ls __ls__ : creates a symbolic link to /bin/ls, named __ls__.
cp -nu *.html .. : copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.  
