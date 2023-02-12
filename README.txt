Practicing git and github 

This repo was created as a place to practice git commands.
It also serves as a reference for useful commands 

UNSTAGE A COMMIT!

git reset HEAD~1
the 1 can be replaced to reflect the number of commits youd like to go back


INIT
. create local repo with "git init"

REMOTE ADD ORIGIN
. connect local repo to github repo using "git remote add origin https...."

GIT ADD/COMMIT
.use "git add <filename>" to add file to staging area 
."git add . " stages all changes
."git commit -m "message" commits the changes
.make sure to provide a thorough and useful message
. if a file has been previously added and is now modified, use " git commit -am "message"

CHECKOUT / CHECKOUT -B
. use  "git checkout" to see your branches
. add a branch using " git checkout -b <branchname>

GIT DIFF
. use "git diff <branchname> " to compare changes

PUSHING/MERGING A BRANCH
. create a github repo for your branch with " git push -u origin <samebranchname> (same as local branch name)
. on github, click the "compare and pull request"  button
.  create comment about changes and press "create pull request" button
. changes are reviewed, comments can be added to specific lines of code.
. if you have permissions, click "Merge Pull Request" 

DELETE BRANCH
. Once you have finished working in a branch, use " git branch -d <branchname> " to delete. 

MERGE CONFLICTS:
. make sure to merge with master while working on a branch in order to stay up to date
.if changes have been made to master while you were working on a branch, you will have a merge conflict.
this is a change on conflictbranch
this is a change on master, ok? 
(use vscode to keep both changes or choose between them)

GIT RESET
. if you accidently add a file with a mistake, use " git reset". the file will be unstaged.
. if you accidentally commit a file with a mistake, use " git reset HEAD~1 " 
. in git, HEAD is a pointer to the last commit. ~1 means go back one commit.

GIT LOG
. if you need to go back several commits, use " git log "
. log will give you a list of commits with hash codes. use git reset <hashcode> to unstage after this commit
."git reset --hard <hashcode> will not only unstage, but remove as well

FORKING
.forking is creating a copy of a repository. it happens on github. 
.you might fork a repo you do not have permissions in so that you can make your own changes.
