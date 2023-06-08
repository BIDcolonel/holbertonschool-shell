0-current_working_directory - Prints the absolute path name of the current working directory // pwd

1-listit - Display the contents list of your current directory // ls

2-bring_me_home - Changes the working directory to the user’s home directory // cd

3-listfiles - Display current directory contents in a long format // ls -l

4-listmorefiles - Display current directory contents, including hidden files (starting with .). Use the long format // ls -la

5-listfilesdigitonly - Display current directory contents. Long format with user and group IDs displayed numerically And hidden files (starting with .) // ls -lna

6-firstdirectory - Creates a directory named holberton in the /tmp/ directory // mkdir /tmp/my_first_directory

7-movethatfile - Move the file betty from /tmp/ to /tmp/holberton // mv /tmp/betty /tmp/my_first_directory

8-firstdelete - Delete the file betty. The file betty is in /tmp/holberton // rm /tmp/my_first_directory/betty

9-firstdirdeletion - Delete the directory holberton that is in the /tmp directory // rm -r /tmp/my_first_directory

10-back - Changes the working directory to the previous one // cd -

11-lists - Lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format // ls -al . .. /boot

12-file_type - Prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script // file /tmp/iamafile

13-symbolic_link - Create a symbolic link to /bin/ls, named ls. The symbolic link should be created in the current working directory // ln -s /bin/ls __ls__

14-copy_html - Copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory // cp -u *.html ../

15-lets_move - Moves all files beginning with an uppercase letter to the directory /tmp/u // mv [A-Z]* /tmp/u

16-clean_emacs - Deletes all files in the current working directory that end with the character ~ // rm *~

17-tree - Creates the directories welcome/, welcome/to/ and welcome/to/holberton in the current directory // mkdir -p welcome/to/school
