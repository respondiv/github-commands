###### create git repository within a directory. The 1st first Step 

`git init`


###### see the status of the repository

`git status`


###### log of every commit ever made

`git log`


###### log of every commit with stats

`git log --stat`


press `q` to quit git log output screen


###### Add a file to staging area

`git add file_name`

or for multiple filename

`git add file_name1 file_name2 file_name3`

or for all file

`git add *`  or  `git add .`


###### remove a file from staging area

`git reset file_name`


###### discard any changes either(both) on working directory or staging area (be very careful when running this command)

`git reset --hard`


###### commit the changes and specify commit message (normally do one commit per logical change)

`git commit`

or (this is shortcut)

`git commit -m "Commit Message" `


###### if you want to compare the files from working directory and staging area (when there is no commit id)

`git diff`


###### if you want to compare the files from staging area and Repository 

`git diff --staged`


###### compares different versions of file

`git diff commit_id_1 commit_id_2`


###### Switch branches / work / restore previous (any) versions of file

`git checkout commit_id`

or

`git checkout branch-name`


###### display the list of brances for repository

`git branch`


###### create a new branch from master

`git branch new_branch_name`


###### view the commit history between different branched in one place (e.g master and branch1)

`git log --graph --oneline master branch1`


###### If you are checking out a commit id (say to pinpoint a bug) and want to crate a branch from that commit id so that your work won't be lost, use following (it's a combination of using git checkout and git branch command)

`git checkout -b new_branch_name`


###### run git garbage collection (delete all unused / unreachable commits)

`git gc`


```
Note: Merge 2 or more branch. Always checkout the branch that you want other to merge and point. (say you are merging a master and branch1 and want branch1 to merge and point to master then do "git checkout master" before running the merge command, if you are merging and pointing master to branch1 then do "git checkout branch1" before running the merge command)

Git merge will also include the currently checked-out branch in the merged version. So if you have branch1 checked out, and you run "git merge branch2 branch3", the merged version will combine branch1 as well as branch2 and branch3. For this reason, you should always checkout one of the two (or more) branches you’re planning on merging before doing the merge. Which one you should check out depends on which branch label you want to point to the new commit.
```


###### Merge 1 or more branch

`git merger master branch1`

or 

`git merge branch1 branch2`


###### if there is merge error and want to abort the merge use git merge --abort and then use git log and or git diff find the issue, fix it and redo the merge process

`git merge --abort`


###### comparing a commit to it's parent without knowing parent id

`git show commit_id`


###### delete a unnecessary git branch(say after merging)

`git branch -d branch_name`


###### view all the remote repository

`git remote`


###### add a remote repository (e.g from github), if you only have 1 remote name it origin

`git remote add remote_name url_for_git_with_https`

e.g

`git remote add origin https://github.com/repository.git`


###### verify the added remote

`git remote -v`


###### send (push) the chages to the repository (remote)

`git push -u remote_name branch_name_you_want_to_push`

e.g 

`git push -u origin master`


###### receive (pull) the changes from github (remote) to local computer

`git pull remote_name branch_name_you_want_to_pull`

e.g 

`git pull origin master`


###### Forking a Repository: Use github via browser and click Fork button


###### copy / clone the entire repository from remote (initial). Cloning a repository automatically create remote for push and pull

`git clone url_of_repository`


###### Git Fetch will only fetch the code from repository but doesn't merge it to local copy. This will help you to see the difference in coe (conflicts) by doing git log and git diff

`git fetch remote_name`

e.g.

`git fetch origin`


Note: `git pull origin master` = `git fetch origin` and `git merge master origin/master`

