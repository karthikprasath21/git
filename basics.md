# Git Commands

## Basic Commands
- **Git --version**  
  To check version
- **Git init**  
  To initialize a folder for using git
- **Git status**  
  To know current state of current repository
- **Git add .**  
  To add all files in present directory
- **Git commit -m "message"**  
  Commit with commit message
- **git commit --amend**  
  Can save you if you have made a mistake in previous commit (just previous one)

## Viewing History
- **Git log**  
  To view the commit history
- **git log --oneline**  
  To view commit history in one line

## Configuration
- **git config --global core.editor "code --wait"**  
  To make VS Code as default editor

## Ignoring Files
- **.gitignore**  
  Add this file to specify the file/folder to avoid from being tracked from git. Patterns can also be used to specify things to be avoided.

## Branching
- **Git branch**  
  To view the existing branches
- **Git branch name**  
  To create a new branch
- **Git switch name**  
  To switch to specified branch
- **Git switch -c name**  
  To create and switch to specified branch
- **Git checkout**  
  Same as Git switch
- **Git checkout -b name**  
  Same as Git switch -c name
- **Git branch -d name**  
  To delete a branch
- **Git branch -D name**  
  To delete a branch forcefully
- **git branch -m name newname**  
  Stay in this branch while renaming this branch

## Merging
- **Git merge name**  
  To merge a branch. Stay in the branch where you wanted to perform merge.

## Comparing Changes
- **Git diff**  
  Compares file between staging area & current working directory
- **Git diff HEAD**  
  Compares file between all last commit & current working directory
- **Git diff --staged/--cached**  
  Compares file between last commit & current staging area
- **Git diff branch1..branch2**  
  Compare all changes between 2 branches which are committed
- **Git diff commit1..commit2**  
  Compare all changes between 2 commits

## Stashing
- **Git stash**  
  To save the changes in a temporary location without add or commit
  - **--save** (optional)
- **Git stash pop**  
  To apply the saved stash to existing branch but only once (like ctrl+x ctrl+v)
- **Git stash apply**  
  To apply the saved stash
- **Git stash apply**  
  To apply the saved stash to any existing branch (like ctrl+c ctrl+v)
- **Git stash list**  
  To list all stashed code
- **Git stash apply 'stash@{0}'**  
  To implement the specific stash
- **Git stash drop 'stash@{0}'**  
  To delete specific stash
- **Git stash clear**  
  To delete all stash in list

## Switching Branches
- **Git switch branch**  
  To reattach our head to top of the commit, if our head was detached before due to git checkout in earlier commits
- **Git switch -**  
  Same as Git switch branch

## Checking Out
- **Git checkout HEAD~1**  
  To go to previous commit
- **Git checkout HEAD filename**  
  To discard the changes newly made before committed or staged. It takes us to last commit of the specific file
- **Git checkout -- filename**  
  To discard the changes newly made before committed or staged. It takes us to last commit of the specific file

## Restoring
- **Git restore filename**  
  Same as Git checkout HEAD filename / Git checkout -- filename
- **Git restore --source HEAD~1 filename**  
  Same as Git checkout HEAD~1
- **Git restore --staged filename**  
  To remove from staging area

## Resetting
- **Git reset #0000**  
  To reset to specific commit. The new changes will still exist, if required they can be saved in new branch
- **Git reset --hard #0000**  
  Similar to Git reset #0000 but this will not hold the new changes

## Reverting
- **Git revert #0000**  
  Similar to git reset but it will create a new commit having the history of newer things, but we will be reverted back to our desired point# Git Commands

## Basic Commands
- **Git --version**  
  To check version
- **Git init**  
  To initialize a folder for using git
- **Git status**  
  To know current state of current repository
- **Git add .**  
  To add all files in present directory
- **Git commit -m "message"**  
  Commit with commit message
- **git commit --amend**  
  Can save you if you have made a mistake in previous commit (just previous one)

## Viewing History
- **Git log**  
  To view the commit history
- **git log --oneline**  
  To view commit history in one line

## Configuration
- **git config --global core.editor "code --wait"**  
  To make VS Code as default editor

## Ignoring Files
- **.gitignore**  
  Add this file to specify the file/folder to avoid from being tracked from git. Patterns can also be used to specify things to be avoided.

## Branching
- **Git branch**  
  To view the existing branches
- **Git branch name**  
  To create a new branch
- **Git switch name**  
  To switch to specified branch
- **Git switch -c name**  
  To create and switch to specified branch
- **Git checkout**  
  Same as Git switch
- **Git checkout -b name**  
  Same as Git switch -c name
- **Git branch -d name**  
  To delete a branch
- **Git branch -D name**  
  To delete a branch forcefully
- **git branch -m name newname**  
  Stay in this branch while renaming this branch

## Merging
- **Git merge name**  
  To merge a branch. Stay in the branch where you wanted to perform merge.

## Comparing Changes
- **Git diff**  
  Compares file between staging area & current working directory
- **Git diff HEAD**  
  Compares file between all last commit & current working directory
- **Git diff --staged/--cached**  
  Compares file between last commit & current staging area
- **Git diff branch1..branch2**  
  Compare all changes between 2 branches which are committed
- **Git diff commit1..commit2**  
  Compare all changes between 2 commits

## Stashing
- **Git stash**  
  To save the changes in a temporary location without add or commit
  - **--save** (optional)
- **Git stash pop**  
  To apply the saved stash to existing branch but only once (like ctrl+x ctrl+v)
- **Git stash apply**  
  To apply the saved stash
- **Git stash apply**  
  To apply the saved stash to any existing branch (like ctrl+c ctrl+v)
- **Git stash list**  
  To list all stashed code
- **Git stash apply 'stash@{0}'**  
  To implement the specific stash
- **Git stash drop 'stash@{0}'**  
  To delete specific stash
- **Git stash clear**  
  To delete all stash in list

## Switching Branches
- **Git switch branch**  
  To reattach our head to top of the commit, if our head was detached before due to git checkout in earlier commits
- **Git switch -**  
  Same as Git switch branch

## Checking Out
- **Git checkout HEAD~1**  
  To go to previous commit
- **Git checkout HEAD filename**  
  To discard the changes newly made before committed or staged. It takes us to last commit of the specific file
- **Git checkout -- filename**  
  To discard the changes newly made before committed or staged. It takes us to last commit of the specific file

## Restoring
- **Git restore filename**  
  Same as Git checkout HEAD filename / Git checkout -- filename
- **Git restore --source HEAD~1 filename**  
  Same as Git checkout HEAD~1
- **Git restore --staged filename**  
  To remove from staging area

## Resetting
- **Git reset #0000**  
  To reset to specific commit. The new changes will still exist, if required they can be saved in new branch
- **Git reset --hard #0000**  
  Similar to Git reset #0000 but this will not hold the new changes

## Reverting
- **Git revert #0000**  
  Similar to git reset but it will create a new commit having the history of newer things, but we will be reverted back to our desired point
