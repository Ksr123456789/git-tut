what is vim editor

Note while you do `git commit` after that vim editor opens, so firstly then click 'i' and then after write commit message then after that click esc , which is located in upper left area of keyboard after that write ":wq" and press enter

1.  `git init` -> powers your folder to be managed by git, and initalises a new empty repositary. It also creates a .git folder that has all the relevant logic to manage versions of your project. If we again give git init command then it will reinitalized the existing git repositary

2.  `working area` --> There can be bunch of files that are not currently handled by git. It means that changes done or to be done in those files are not managed by git yet. A file which is in working area is considered to be not in the staging area. When we do `git status` and we see a bunch of `untracked files` then these are actullay called to be in the working area

3.  `staging area` --> staging area tells what all files are going to be part of the next version that we will create. this staging area is the place where git knows what changes will be done from the last version to the next version

4.  `repositary Area` -> This area actually contains the details of all your previous registered versions. and the files in this area, git already manages them and knows their version history

5.  `git add <file>` is used to move file from working area to staged area
6.  `git rm --cached <file>` is used to move file from staged area back to working area

7.  `commit` --> commit is a particular version of a project, it captures a snapshot of the project's staged changes and creates a version out of it.

8.  `git commit` -->registers staging changes to a commit

9.  `git log` --> list downs all the commits of the repositary. if you want to exit out of git log prompt press 'q'

10. `git restore <file>` --> it remove all files changes from the staging area to be committed. this can be useful if we wrote some dirty piece of code and now no more want it. Instead of deleting every change line by line we can use `git restore` and it will restore last clean version of the file.

11. `git restore --staged <file>` --> it move back the file changes from staging area to the working area.
    this only works if changes are in your staging area

12. Diff between git rm and git restore
    ans: if you want to move the whole file back to the untracked state(working state), then we do git rm, otherwise if we just want to remove the changes in working area then we do git restore.

13. `git diff commit1 commit2` --> gives the difference of all file changes between two commits

14. `git commit -m <"your commit message">` --> if we want to avoid opening a text editor line vim/nano to add commit message we can use this following command

15. `git remote` --> list down all the remote connection names

    here remote means which is present somewhere else

16. Remote connection --> link two git repositaries for uploading and downloading changes from each other

17. `git remote add <name of remote> <link of remote>` --> this command helps us to add a new link to the remote repo and give a name to it

18. `git remote rm <name of remote>` : this command deletes remote connection

19. `git remote rename <oldname> <newname> : this command renames the remote connection

NOTE :- The name of the remote connection is always used to establish communication between the repos

20. `git add <file1> <file2> <file3>` : this command will add multiple file changes together in the staging area

21. `git add .` --> this command will add all commands from working repo to the staging area.

22. `git pull <remote name> <branch name>` --> downloads latest changes from the branch of the mentioned remote in your local repo.

### recommended practice to do

-make changes
-git add <file>
-git commit
-git pull
-git push

merge conflicts can occur if multiple people try to make changes to the same file and then collaborate.
