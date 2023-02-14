Shell Variables Expansions

alias ls="rm *" : script that creates an alias.
echo hello $USER : prints hello user, where user is the current Linux user.
PATH=$PATH:/action : Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.
echo $PATH | tr ":" "\n" | wc -l : counts the number of directories in the PATH.
printenv : script that lists environment variables.
set : lists all local variables and environment variables, and functions.
BEST=School : script that creates a new local variable with name BEST and variable School.
export BEST=School : script that creates a new global variable.
echo $((TRUEKNOWLEDGE+128)) : script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE.
echo $((POWER/DIVIDE)) : prints the result of POWER divided by DIVIDE.
echo $((BREATH**LOVE)) : displays the result of BREATH to the power LOVE.
