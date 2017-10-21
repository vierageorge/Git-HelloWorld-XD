# Git-HelloWorld-XD
This is where I, finally, decide to start learning Git

This my initial Git cheat sheet that I'll be, probably, updating once in a while.

1. Create a directory in PC. This will be the working directory.
2. Goto working directory and
>> git init
This will start a new repository.

3. Clone a repo. Alternatively you can clone a repo that's in another place in your PC or even a remote repo (like, the ones in Github.)
>> git clone /path/to/repo
or
>> git clone https://github.com/....

4. To add a file to the staging index
>> git add FILE_NAME
or to add a all files with changes to the staging index
>> git add .

5. To reverse changes in a file that has not been added to the staging index.
>> git checkout -- FILE_NAME

6. To confirm changes in staging index:
>> git commit
Write a message describing the commit. First name, summary; next paragraph descriptive.

7. Usefull commands to check status and logs
>> git status
>> git log
>> git log --oneline
>> git log --oneline --decorate

8. To upload branch to remote repository, fist, you add your remote repo:
>> git remote add origin REMOTE_PATH (i.e.: https://github...)
Upload branch
>> git push origin BRANCH_NAME (i.e.: master)

10. You can erase a file from your working directory. After that:
>> git rm FILE_NAME
>> git commit
It is not recommended to erase files.

11. Once you've added a file to the staging index, you can remove it from there with:
>> git reset HEAD FILE_NAME

12. To create a branch and start working in it:
>> git checkout -b BRANCH_NAME

13. To erase a branch:
>> git branch -d BRANCH_NAME

14. And to erase it from the remote repository:
>> git push origin :BRANCH_NAME

15. To merge two branches, switch to the destination branch:
>> git checkout DEST_BRANCH (i.e.: master)
Then
>> git merge ORG_BRANCH
(ORG_BRANCH, the branch that has the changes you want to bring to your destination branch)

16. To check the status of and old commit
>> git checkout COMMIT_CODE
This code you can take it from "git log"

17. You can add tags to commits:
Add a TAG to the current commit
>> git tag TAG
Add a TAG to a previous commit
>> git tag TAG COMMIT_CODE
