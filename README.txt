what is vim editor

Note while you do `git commit` after that vim editor opens, so firstly then click 'i' and then after write commit message then after that click esc , which is located in upper left area of keyboard after that write ":wq" and press enter

1.  `git init` -> powers your folder to be managed by git, and initalises a new empty repositary. It also creates a .git folder that has all the relevant logic to manage versions of your project. If we again give git init command then it will reinitalized the existing git repositary


2.  `working area` --> There can be bunch of files that are not currently handled by git. It means that changes done or to be done in those files are not managed by git yet. A file which is in working area is considered to be not in the staging area. When we do `git status` and we see a bunch of `untracked files` then these are actullay called to be in the working area

3.  `staging area` --> staging area tells what all files are going to be part of the next version that we will create. this staging area is the place where git knows what changes will be done from the last version to the next version 
 


4. `repositary Area` -> This area actually contains the details of all your previous registered versions. and the files in this area, git already manages them and knows their version history

5. `git add <file>` is used to move file from working area to staged area
6. `git rm --cached <file>` is used to move file from staged area back to working area

7. `commit` --> commit is a particular version of a project, it captures a snapshot of the project's staged changes and creates a version out of it.

8. `git commit` -->registers staging changes to a commit

9. `git log` --> list downs all the commits of the repositary. if you want to exit out of git log prompt press 'q'

10. `git restore <file>` --> it remove all files changes from the staging area to be committed. this can be useful if we wrote some dirty piece of code and now no more want it. Instead of deleting every change line by line we can use `git restore` and it will restore last clean version of the file.

11. `git restore --staged <file>` --> it move back the file changes from staging area to the working area.
this only works if changes are in your staging area

12. Diff between git rm and git restore
ans: