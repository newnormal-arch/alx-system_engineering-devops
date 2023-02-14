Shell Variables Expansions

alias ls="rm *" : script that creates an alias.
echo hello $USER : prints hello user, where user is the current Linux user.
PATH=$PATH:/action : Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.
echo $PATH | tr ":" "\n" | wc -l : counts the number of directories in the PATH.
