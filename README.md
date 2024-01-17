
### Setting up Git configurations
| Command | Description |
| ------- | ----------- |
| `git config --global user.name "Your Name"` | Sets the name that will be attached to your commits and tags. |
|`git config --global user.email "your@email.com" `| Sets the email address that will be attached to your commits and tags.|
|` git config user.name`| Checking the configured user name|
|`git config user.email`|Checking the configured user email|
|`git config --list`|Lists all the Git configuration settings.|

### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `mkdir my_repo` | Creating a new directory for the repository |
| `cd my_repo` | Navigating into the directory |
| `git init` | Initializing a new Git repository  |
| `git clone <remote_url>` | Cloning a repository from a remote URL |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |


![image](https://github.com/amer787/Git-Commands-/assets/46135816/5e3d54bf-b37d-40af-8cc7-72f305139b5d)

### Checkout
| Command | Description |
| ------- | ----------- |
| `git checkout <branch>` | Switches to a different branch. |
| `git checkout <commit>` | Moves to a specific commit in "detached HEAD" state. |
| `git checkout -- <file>` | Discards changes in the working directory for a specific file. |

### Reverting
| Command | Description |
| ------- | ----------- |
| `git revert <commit>` | Purpose: Used to create a new commit that undoes the changes made by a specific commit. |

### Resetting
| Command | Description |
| ------- | ----------- |
| `git reset --soft <commit>` | Moves the HEAD and branch pointer to a specific commit, keeping changes staged. |
| `git reset --mixed <commit>` | Moves the HEAD and branch pointer to a specific commit, unstaging changes. |
| `git reset --hard <commit>` | Moves the HEAD and branch pointer to a specific commit, discarding changes in the working directory. |




### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add .` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit changes |
| `git commit --amend -m "[commit message]"` | Change a commit with a message |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |
| `git rm --cached <file-name>` | Removing a file from the staging area |
| `git reset <file-name>` | Resetting changes of a file in the working directory to the last committed state |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git branch -m [old branch name] [new branch name]` | Rename a local branch |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log --oneline` | View changes (briefly) |
| `git diff [source branch] [target branch]` | Preview changes before merging |
