Shell I/0 Redirections and Filters

echo -e Hello, World : prints “Hello, World”, followed by a new line to the standard output.
echo -e \"\(\Ôo\)\' : script that displays a confused smiley "(Ôo)'.
cat /etc/passwd : Display the content of the /etc/passwd file.
cat /etc/passwd /etc/hosts : Display the content of /etc/passwd and /etc/hosts.
tail -n 10 /etc/passwd : Display the last 10 lines of /etc/passwd.
head -n 10 /etc/passwd : Display the first 10 lines of /etc/passwd.
head -3 iacta | tail -1 : displays the third line of the file iacta.
echo "Best School" > \\\*\\\\\'\"Best\ School\"\\\'\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*\:\) : creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line.
ls -la > ls_cwd_content : writes into the file ls_cwd_content the result of the command ls -la.
tail -1 iacta >> iacta : script that duplicates the last line of the file iacta.
find . -name \*.js -type f -delete :  deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders.
find . -mindepth 1 -type d | wc -l : counts the number of directories and sub-directories in the current directory.
ls -1 -t | head -10 : displays the 10 newest files in the current directory.
sort | uniq -u : takes a list of words as input and prints only words that appear exactly once.
grep root /etc/passwd : Display lines containing the pattern “root” from the file /etc/passwd.
grep bin /etc/passwd | wc -l : Display the number of lines that contain the pattern “bin” in the file /etc/passwd.
grep -A 3 root /etc/passwd : Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.
grep -v bin /etc/passwd : Display all the lines in the file /etc/passwd that do not contain the pattern “bin”.
grep ^[[:alpha:]] /etc/ssh/sshd_config : Display all lines of the file /etc/ssh/sshd_config starting with a letter.
tr A Z | tr c e : Replace all characters A and c from input to Z and e respectively.
tr -d Cc :  removes all letters c and C from input.
rev : script that reverse its input.
cut -d":" --fields=1,6 /etc/passwd | sort : displays all users and their home directories, sorted by users.
find . -empty -printf "%f\n" : finds all empty files and directories in the current directory and all sub-directories.
find . -type f -name \*.gif -printf "%f\n" | LC_ALL=C sort -f | rev | cut -b 5- | rev : lists all the files with a .gif extension in the current directory and all its sub-directories.
echo $(cut -b 1 | tr -d '\n') : script that decodes acrostics that use the first letter of each line.
tail -n+2 | cut -f1 | sort | uniq -c | sort -rn | cut -c 9- | head -11 : cript that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.
