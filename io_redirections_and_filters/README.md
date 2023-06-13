Shell , I/O redirections and filters

0-hello_world : prints “Hello, World”, followed by a new line to the standard output // echo "Hello, World"

1-confused_smiley : displays a confused smiley "(Ôo)' // echo "\"(Ôo)'"

2-hellofile : Display the content of the /etc/passwd file // less /etc/passwd

3-twofiles : Display the content of /etc/passwd and /etc/hosts // less /etc/passwd /etc/hosts

4-lastlines : Display the last 10 lines of /etc/passwd // tail -n 10 /etc/passwd

5-firstlines : Display the first 10 lines of /etc/passwd // head -n 10 /etc/passwd

6-third_line : Displays the third line of the file iacta -You’re not allowed to use sed // head -n 3 iacta | tail -n 1

7-file : Creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line // echo "Best School" > \\\*\\\\"'\"Best School\"\\'"\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*\:\)

8-cwd_state : Writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it // ls -la > ls_cwd_content

9-duplicate_last_line : Duplicates the last line of the file iacta // tail -n 1 iacta >> iacta

10-no_more_js : Deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders // find . -type f -name "*.js" -delete

11-directories : counts the number of directories and sub-directories in the current directory -The current and parent directories should not be taken into account -Hidden directories should be counted // find . -mindepth 1 -type d | wc -l

12-newest_files : Displays the 10 newest files in the current directory -One file per line -Sorted from the newest to the oldest // ls -1t | head

13-unique : Takes a list of words as input and prints only words that appear exactly once -Input format: One line, one word -Output format: One line, one word -Words should be sorted // sort | uniq -u

14-findthatword : Display lines containing the pattern “root” from the file /etc/passwd // grep -e "root" /etc/passwd

15-countthatword : Display the number of lines that contain the pattern “bin” in the file /etc/passwd // grep -c bin /etc/passwd

16-whatsnext : Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd // grep -A 3 root /etc/passwd

17-hidethisword : Display all the lines in the file /etc/passwd that do not contain the pattern “bin” // grep -not bin /etc/passwd

18-letteronly : Display all lines of the file /etc/ssh/sshd_config starting with a letter -include capital letters as well // grep ^[a-zA-Z] /etc/ssh/sshd_config

19-AZ : Replace all characters A and c from input to Z and e respectively // tr  "A" "Z" | tr "c" "e"

20-hiago : Create a script that removes all letters c and C from input // tr -d "c" | tr -d "C"

21-reverse : Write a script that reverse its input // rev

22-users_and_homes : Write a script that displays all users and their home directories, sorted by users -Based on the the /etc/passwd file // cat /etc/passwd | cut -d: -f1,6 | sort
