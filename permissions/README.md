Shell permission

0-iam_betty : switches the current user to the user betty // su betty

1-who_am_i : prints the effective username of the current user // whoami

2-groups : prints all the groups the current user is part of // groups

3-new_owner : changes the owner of the file hello to the user betty // chown betty hello

4-empty : creates an empty file called hello // touch hello

5-execute : adds execute permission to the owner of the file hello // chmod u+x hello

6-multiple_permissions : adds execute permission to the owner and the group owner, and read permission to other users, to the file hello // chmod ug+x,o+r hello

7-everybody : adds execution permission to the owner, the group owner and the other users, to the file hello // chmod ugo+x hello

8-James_Bond : sets the permission to the file hello as follows: -Owner: no permission at all -Group: no permission at all -Other users: all the permissions // chmod 007 hello

9-John_Doe : sets the mode of the file hello to this: -rwxr-x-wx // chmod 753 hello

10-mirror_permissions : sets the mode of the file hello the same as olleh’s mode // chmod --reference=olleh hello

11-directories_permissions : adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed // chmod -R +X .
