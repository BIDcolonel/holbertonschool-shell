Shell, init files, variables and expansions

0-alias : Creates an alias -Name: ls -Value: rm * // alias ls="rm *"

1-hello_you : Prints hello user, where user is the current Linux user // echo hello $USER

2-path : Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program // export PATH="$PATH:/action"

3-paths : Counts the number of directories in the PATH // echo $PATH | tr ":" "\n" | wc -l

4-global_variables : Lists environment variables // printenv

5-local_variables : Lists all local variables and environment variables, and functions // set

6-create_local_variable : Creates a new local variable -Name: BEST -Value: School // BEST=School

7-create_global_variable : Creates a new global variable -Name: BEST -Value: School // export BEST=School

8-true_knowledge : Prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line // echo "$((128+TRUEKNOWLEDGE))"

9-divide_and_rule : Prints the result of POWER divided by DIVIDE, followed by a new line -POWER and DIVIDE are environment variables// echo "$((POWER/DIVIDE))"

10-love_exponent_breath : Displays the result of BREATH to the power LOVE -BREATH and LOVE are environment variables -The script should display the result, followed by a new line // echo "$((BREATH**LOVE))"

11-binary_to_decimal : onverts a number from base 2 to base 10 -The number in base 2 is stored in the environment variable BINARY -The script should display the number in base 10, followed by a new line // echo $((2#$BINARY))

12-combinations : Prints all possible combinations of two letters, except oo -Letters are lower cases, from a to z -One combination per line -The output should be alpha ordered, starting with aa -Do not print oo -Your script file should contain maximum 64 characters // echo {a..z}{a..z} | tr " " "\n" | grep -v "oo"

13-print_float : Prints a number with two decimal places, followed by a new line -The number will be stored in the environment variable NUM // echo $(printf %.2f $NUM)

14-decimal_to_hexadecimal : Converts a number from base 10 to base 16 -The number in base 10 is stored in the environment variable DECIMAL -The script should display the number in base 16, followed by a new line // echo $(printf '%x\n' $DECIMAL)
