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

## If Local Repo is created first, but remote is not
* 1.	First Create a remote repository at github/ bitbucket
* 2.	git remote add git-command https://github.com/codehub7/git-command.git
    * git remote add <remote_name> <remote_repo_url>
* 3.	git push -u git-command master
    * git push -u <remote_name> <local_branch_name>
