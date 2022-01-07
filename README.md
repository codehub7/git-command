# git-command
## Git Command Cheat Sheet
* git init
* git add file_name.extention
* git add .   (add all files to staging area)
* git commit -m “message” filename.ext (single file can be mentioned)
* git commit -am "message"   (all file changes will be commited)
* git commit --amend
* git status
* git log
* git log --reflog
* git config –global alias.co checkout

* git show hash_of_commit
    * example: git show ed59633
* git checkout hash_of_commit ( go back to that commit )
  * git checkout master ( go back to master branch again)
* git checkout hash_of_commit task.txt ( go back to that commit for task.txt file only)
    * git checkout master -f ( if only one file has to go back to master)
* git reset --soft hash_of_commit (doesn't delete any change)
* git reset --hard hash_of_commit (delete all changes)

* git stash 
* git stash save "message of the stash"
* git stash -p (select each of the files if you want to stash it or not)
* git stash list
* git stash pop
* git stash pop "stash@{1}"
* git stash clear
* git stash drop "stash@{1}"
* git clean -f (remove all untracked files)
* git clean -f -n (dry run to clear all untracked files)
<br><br>
* git log 
* git log --oneline
* git log --stat
* git log filename.extention
* git log -n number_of_commit_want_to_show (ex: git log -n 3 will show 3 recent commits)

## If Local Repo is created first, but remote is not
* 1.	First Create a remote repository at github/ bitbucket
* 2.	git remote add git-command https://github.com/codehub7/git-command.git
    * git remote add <remote_name> <remote_repo_url>
* 3.	git push -u git-command master
    * git push -u <remote_name> <local_branch_name>
