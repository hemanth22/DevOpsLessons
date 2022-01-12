# Git Cheat List

## Project Workflow

Git command to initialize any project:
  ```
  $git init
  ```
Command to add changes:
  ```
  $git add -A
  ```
  *or*
  ```
  $git add .
  ```
  *or*
  ```
  $git add filename.extension
  ```
Command to commit changes:
  ```
  $git commit -m "Commit Message"
  ```
Command to create repository
  ```
  $git create
  ```
Command to push changes:
  ```
  $git push
  ```
  *or*
  ```
  $git push origin
  ```
  *or*
  ```
  $git push origin branch_name
  ```
command to push the changes forcefully:
  ```
  $git push -f
  ```
## Logs

Command to get the log of the repository:
  ```
  $git log
  ```
  *or*
  ```
  $git log -n 1
  ```
  *or*
  ```
  $git log –-since=2017-01-21
  ```
  *or*
  ```
  $git log –-until=2017-01-22
  ```
  *or*
  ```
  git lg -p
  ```
  *or*
  ```
  $git log –-grep="Init"
  ```
## Help command

Command to get help of command:
  ```
  $git help command
  ```
  __**Example:**__:
  ```
  $git help log
  ```
  __**Git Command to check log of individual file**__
  ```
  $git log -- [filename]
  ```
  __**Use --follow option in git log to view a file's history**__
  ```
  $git log --stat -p -- src/somefile.ts
  ```
## Status commands

Command to check to status of repository:
  ```
  $git status
  ```
  *or*
  ```
  $git status -s
  ```

## Diff commands
  
Command to check difference in the repository:
  ```
  $git diff
  ```
  *or*
  ```
  $git diff filename
  ```
  *or*
  ```
  $git diff --staged
  ```
  *or*
  ```
  $git diff --cached
  ```
## Delete / Renaming commands
  
Command to delete filename:
  ```
  $git rm filename
  ```
Command to delete filename from staged or cached index:
  ```
  $git rm --cached
  ```
Command to rename filename:
  ```
  $git mv filename newfilename
  ```
## Undo changes

  ```
  $git checkout -- <file>
  ```
  -- indicates current branch

## Unstage changes
   ```
   $git reset HEAD <file>
   ```
## Undoing change amending commits.
  ```
  $git commit --amend -m “Previous comment message copy and paste here.”
  ```
## Old Version undoing changes – reverting a commit 
  ```
  $git checkout lastcommitchecksum -- <file> 
  ```
  -- means present directory

  lastcommitchecksum means there will checksum every commit that needs to be placed here

## New Version undoing change – reverting a commit
  ```
  $git revert lastcommitchecksum
  ```
  It will pop-up in a file, then save and exit


## Undoing change - - using reset commit
  
  Soft reset commit
  ```
  $git reset --soft commitchecksum
  ```
  Mixed reset commit
  ```
  $git reset --mixed commitchecksum
  ```
  Hard reset commit
  ```
  $git reset --hard commitchecksum
  ```
  
## Undoing Changes – Removing Untrack
  ```
  $git clean
  ```
  ```
  $git clean -n
  ```
  
## Git ignore 
  ```
  $touch .gitignore
  ```
  .gitignore 
  
  It is used to ignore files which you mention in .gitignore

  ```
  $git config –global core.excludesfile ~/.gitignore_global
  ```

## To remove file from staging or cached index
  ```
  $git rm --cached <file>
  ```
to track the empty directory put .gitkeep in the empty directory

## How to get commit tree of HEAD
  ```
  $git ls-tree HEAD
  ```
  ```
  $git ls-tree master
  ```
## To know seperate directory HASH Commit
  ```
  $git ls-tree master [directory]
  ```
## How to see HASH of file inside the directory using HASH Commit
  ```
  $git ls-tree SHACODE#[min 10character]
  ```
## More tricks on git commit log
  ```
  $git log --oneline
  ```
  ```
  $git log --oneline -3
  ```
  ```
  $git log --since="2017-01-26"
  ```
  ```
  $git log --since="2 weeks ago" --until="3 days ago"
  ```
  ```
  $git log --since=2.weeks --until=3.days
  ```
  ```
  $git log --author="hemanth"
  ```
  ```
  $git log --grep="file"
  ```
  ```
  $git log ca834f5..03b1b6c --oneline
  ```
  ```
  $git log -p
  ```
  ```
  $git log -p ca834f5
  ```
  ```
  $git log --format=oneline
  ```
  ```
  $git log --format=short
  ```
  ```
  $git log --format=full
  ```
  ```
  $git log --format=email
  ```
  ```
  $git log --format=raw
  ```
  ```
  $git log --graph
  ```
  ```
  $git log --oneline --graph --all --decorate
  ```
  ```
  $git show 3c0aff9
  ```
  ```
  $git show --format=oneline HEAD
  ```
  ```
  $git show --format=oneline HEAD^^
  ```
  ```
  $git show --format=oneline HEAD~3
  ```
  ```
  $git show 994170cc939
  ```
## Diff commands
  
  ```
  $git diff 3c0aff9 resources.html
  ```
  ```
  $git diff 3c0aff..HEAD
  ```
  ```
  $git diff 3c0aff..HEAD^^
  ```
  ```
  $git diff --stat --summary 3c0aff9..HEAD
  ```
  ```
  $git diff --ignore-space-change 3c0aff9..HEAD
  ```
  ```
  $git diff --ignore-all-space 3c0aff9..HEAD
  ```
  ```
  $git diff -w 3c0aff9..HEAD
  ```
  ```
  $git branch
  ```
Command to display all local and remote branches

  ```
  $git branch -a
  ```
Command to display only remote branches

 ```
 $git branch -r
 ```
 
## To create new branch 
  ```
  $git branch new_feature
  ```
  new_feature is new branch name

## Switch to new branch 
  ```
  $git checkout new_feature
  ```
## To switch back same code above
  ```
  $git checkout master
  ```
## Create and switch branch at one shot command
  ```
  $git checkout -b <branch_name>
  ```
## Branching – Switching branches with uncommitted changes
  ```
  $git commit -am “Swap out”
  ```
## Comparing git branches
  ```
  $git diff <branch_new>..<branch_new>
  ```
## Comparing git branches with colour
  ```
  $git diff --color-words <branch_new>..<branch_new>
  ```
## Comparing git branches history with colour
  ```
  $git diff --color-words <branch_new>..<branch_new>^
  ```
## Branches which is merged each other
  ```
  $git branch --merged
  ```
## Renaming branches
  ```
  $git branch -m <branch_name> <new_branch_name> (OR)
  ```
  ```
  $git branch --move <branch_name> <new_branch_name>
  ```
## Delete Branch
  ```
  $git branch -d <branch> (OR)
  ```
  ```
  $git branch --delete <branch>
  ```
## Delete Commited Branch
  ```
  $git branch -D <branch>
  ```
## Creatig a pull request
  
  Create and checkout to new_branch
  ```
  $git checkout -b new_branch
  ```
  After any new file and push changes to new_branch 
  ```
  $git push -u origin new_branch
  ```
  create a pull request on new_branch
  ```
  $git pull-request -b project_name:master -h project_name:new_branch
  ```
## Forking a Repo
  
  Clone a repo
  ```
  $git clone deadlyvipers/dojo_rules
  ```
  Change to project repository
  ```
  cd dojo_rules
  ```
  Fork the repo
  ```
  $git fork
  ```
## Updating fork
  
  Add remote for upstream
  ```
  $git remote add upstream <path_to_repo>
  ```
  Fetch changes
  ```
  $git fetch upstream
  ```
  Merge them into master
  ```
  $git merge upstream/master master
  ```
  push to remote
  ```
  $git push origin master
  ```

## Config unix command prompt to show the branch
  ```
  $__git_ps1 (OR)
  ```
  ```
  $export PS1='$(__git_ps1 "(%s)") > '
  ```
## Merge branches
  ```
  $git merge <branch_name>
  ```
  ```
  $git branch --merge <branch_name>
  ```
## Merge without fast forward
  ```
  $git merge --no-ff branch <branch_name>
  ```
## Merge with fast forward
  ```
  $git merge --ff-only branch <branch_name>
  ```
## Merge conflicts

# 1.To Abort merge
  ```
  $git merge --abort
  ```
# 2. To resolve merge conflicts
  ```
  $git mergetool –-tool=gvimdiff
  ```
## Stashing changes Saving changes in the stash
  ```
  $git stash save “Commit message here”
  ```
  ```
  $git stash list # to list out stash
  ```
  ```
  $git stash show stach@{0} #This is similar to git diff
  ```
  ```
  $git stash show -p stach@{0} #this is patch to git diff
  ```
## Stashing changes – Retrieving stashed changes
  ```
  $git stash pop stash@{0}
  ```
  ```
  $git stash apply
  ```
## Stashing changes – Deleting stashed changes
  ```
  $git stash drop stash@{0}
  ```
  ```
  $git stash clear
  ```
  
## Rebase
  
  For Interactive rebase use below command
  ```
  $git rebase -i
  ```
  To create and checkout to feature_banch and update your code here
  ```
  $git checkout -b feature_banch
  ```
  After updating code to rebase you should be in feature branch and use below command to merge in master branch
  ```
  $git rebase master
  ```
  Git rebase example command from old base to new base below  
  ```
  $git rebase --onto <newbase> <oldbase>
  ```
  Another example command  this will rebase master with server branch commit.
  ```
  $git rebase master server
  ```
  
## Git tags

  __Light weight tag__ Just a tag, no message or tagger
  ```
  $git tag
  ```
  __Signed tag__ Uses public key to prove identity of tagger
  ```
  $git tag -s
  ```
  __Annotated tag__ Add info on tagged, when and why
  ```
  $git tag -a
  ```
  **_Example_** 
  ```
  $git tag -a v1.0.0 -m "Tag message"
  ```
  Pushing tags
  ```
  $git push --tags
  ```
  
  ```
  git push origin :tagname
  ```
  ```
  git push --delete origin tagname
  ```
  ```
  git tag --delete tagname
  ```
  
## Git remote 
  ```
  $git remote
  ```
  ```
  $git remote add <alias>
  ```
  ```
  $git remote add origin <github address>
  ```
  ```
  $git remote -v
  ```
  ```
  $git reemote rm origin #to remove remote origin 
  ```
  ```
  $git push -u origin <branch_name>
  ```
  -u is used for tracking file if is not availble it is difficult
  -u similar to --up-stream

## To find remote configuration type as below 
  ```
  $cat .git/config
  ```
## how to find configuration
  ```
  $ls -la .git/refs/remotes/origin/
  ```
  ```
  $ls -la .git/refs/remotes/origin/ -r
  ```
  ```
  $ls -la .git/refs/remotes/origin/ -a
  ```
## Download a clone
  ```
  $git clone <gitlink> <new_directory>
  ```
  ### example
  ```
  $git clone https://github.com/hemanth22/explore_california.git git_version
  ```
## Git API
  
  List of commands
  ```
  $curl https://api.github.com 
  ```
  List of emojis
  ```
  $curl https://api.github.com/emojis
  ```
  public info on user
  ```
  $curl https://api.github.com/users/username
  ```
  A users repos
  ```
  $curl https://api.github.com/users/username/repos
  ```
  Authorization
  ```
  $curl -i -H 'Authorization: token <your_authentication_token>' https://api.github.com/user
  ```
  Create a repo
  ```
  $curl -i -H 'Authorization: token <your_authentication_token>' -d '{"name":"test_repo"}' https://api.github.com/users/repos
  ```

## GIT HUB ARCHITECTURE

  ## Two-Tree architecture

   - Repository
   - working

   ![alt text](https://raw.githubusercontent.com/hemanth22/Images/master/github1.png "Github1")


  ## Three-tree architecture

   ![alt text](https://raw.githubusercontent.com/hemanth22/Images/master/github2.png "Github2")

   “When ever you commit changes you made in the project it generate a checksum.“

  What is check sum

    Checksum algorithm converts data into simple number

    → Same data always equal same checksum

  Checksum algorithm is SHA-1

  Which creates a 40 characters with hexadecimal (0-9,a-f)

  _Example :_  e8be9f76c3e3bf4fa8d06d4aa2ad34428e9c442b

 # HEAD

  pointer to tip of the current branch in repository
  Last state of repository what was last check out  
  
  # Some learnings out of box.  
  
  Command to search keyword in the all the versions of the commit.  

```
git grep "_source" $(git rev-list --all)
git grep "select *" $(git rev-list --all)
git grep "bank" $(git rev-list --all)
```

 Command to give log information in detail.
 
```
git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
```

# If you have a code in local system and if you want to push to github remote repository

```
echo "# GradeBook" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/hemanth22/repositoryname.git
git push -u origin master
```

# Command to fetch issue from commits

```
git log --pretty=oneline | grep -e '[A-Z]\+-[0-9]\+' -o
```

# Command to fetch JIRA tickets from commits

```
git log --pretty=oneline | grep -e 'XON\+-[0-9]\+' -o
```
