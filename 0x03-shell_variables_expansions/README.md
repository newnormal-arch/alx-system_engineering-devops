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
echo $((2#$BINARY)) : script that converts a number from base 2 to base 10.
echo {a..z}{a..z} | tr ' ' '\n' | grep -v oo : script that prints all possible combinations of two letters, except oo.
printf %0.2f'\n' $NUM : prints a number with two decimal places, followed by a new line.
printf %x'\n' $DECIMAL : converts a number from base 10 to base 16.
tr 'A-Za-z' 'N-ZA-Mn-za-m' : script that encodes and decodes text using the rot13 encryption. Assume ASCII.
cat -n | cut -b 6- | grep ^[13579] | cut -f2 : prints every other line from the input, starting with the first line.
printf "%o\n" $(( (5#$(echo $WATER | tr '[water]' '[01234]')) + (5#$(echo $STIR | tr '[stir.]' '[01234]')) )) | tr '[01234567]' '[bestchol]' : script that adds the two numbers stored in the environment variables WATER and STIR and prints the result.
