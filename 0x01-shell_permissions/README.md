Describing what each script is doing:
Task 0:switch the current user to the user betty
file name:0-iam_betty
script:
#!/bin/bash
su betty

Task 1:print the effective username of the current user
file name:1-who_am_i
script:
#!/bin/bash
id -un

Task 2:print all the groups the current user is part of
file name:2-groups
script: 
#!/bin/bash
groups

Task 3:change the owner of the file hello to the user betty
file name:3-new_owner
script:
#!/bin/bash
chown betty hello

Task 4:create an empty file called hello
file name:4-empty
script:
#!/bin/bash
touch hello

Task 5:add execute permission to the owner of the file hello
file name:5-execute
script:
#!/bin/bash
chmod u+x hello

Task 6:add execute permission to the owner and the group owner, and read permission to other users, to the file hello
file name:6-multiple_permissions
script:
#!/bin/bash
chmod u+x,g+x,o+r hello

Task 7:add execution permission to the owner, the group owner and the other users, to the file hello
file name:7-everybody
script:
#!/bin/bash
chmod ugo+x hello

Task 8:sets the permission to the file hello
file name:8-James_Bond
script:
#!/bin/bash
chmod 007 hello

Task 9:sets the mode of the file hello
file name:9-John_Doe
script:
#!/bin/bash
chmod 753 hello

Task 10:set the mode of the file hello the same as olleh’s mode
file name:10-mirror_permissions
script:
#!/bin/bash
chmod --reference=olleh hello

Task 11:add execute permission to all subdirectories of the current directory for the owner, the group owner and all other users
file name:11-directories_permissions
script:
#!/bin/bash
chmod -R ugo+x

Task 12:create a directory called my_dir with permissions 751 in the working directory
file name:12-directory_permissions
script:
#!/bin/bash
mkdir -m 751 my_dir

Task 13:changes the group owner to school for the file hello
file name:13-change_group
script:
#!/bin/bash
chgrp school hello
