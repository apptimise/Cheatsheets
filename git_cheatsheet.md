# Git Terminology
[HEAD](#HEAD) | 

# Git Command List
git [add](#git-add) |
git [clone](#git-clone) |
git [commit](#git-commit) |
git [config](#git-config) |
git [diff](#git-diff) |
git [fetch](#git-fetch) |
git [init](#git-init) |
git [log](#git-log) |
git [pull](#git-pull) |
git [push](#git-push) |
git [remote](#git-remote) |
git [status](#git-status) |

# Git Terminology
## HEAD
HEAD is a pointer to the local branch you’re currently on: <a href="https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell#_switching_branches" target="_blank">Reference</a>

# Git Commands

## Git Basics


### git init
1. Create empty Git repo in specified directory. 
..* Run with no arguments to initialize the current directory as a git repository
```bash 
git init <directory>
```
 
### git clone
Clone repo located at <repo> onto local machine. 
  
Original repo can be located on the local filesystem or on a remote machine via HTTP or SSH.
```bash
git clone <repo>
```

### git config
Define author name to be used for all commits in current repo. 

Devs commonly use --global flag to set config options for current user (configuration values on a global or local project level)
```bash
git config user.name <name>
```

### git add
Stage all changes in <directory> / <file> for the next commit.
  
Replace <directory> with a <file> to change a specific file.
```bash
git add <directory>
```
 
### git commit
Commit the staged snapshot, use <message> as the commit message.
```bash
git commit -m "<message>"
```
 
### git status
List which files are staged, unstaged, and untracked.
```bash
git status
```

### git log
Display the entire commit history using the default format.

For customization see additional options.
```bash
git log
```

### git diff
Show unstaged changes between your index and working directory.
```bash
git diff
```

## Undoing Changes
### git revert
Create new commit that undo all of the changes made in <commit>, then apply it to the current branch.
```bash 
git revert <commit>
```


## Remote Repositories
### git remote 
Create a new connection to a remote repo. Use <name> as a shortcut for <url>

After adding a remote, you can use <name> as a shortcut for <url> in other commands.
```bash 
git remote add <name> <url>
```

### git fetch
Fetch a specific <branch>, from the repo, 

or Leave off <branch> to fetch all remote refs.
```bash 
git fetch <remote> <branch>
```

### git pull
Fetch the specified remote’s copy of current branch and immediately merge it into the local copy
```bash
git pull <remote>
```

### git push 
Push the branch to <remote>, along with necessary commits and objects. 

Creates named branch in the remote repo if it doesn’t exist.
```bash
git push <remote> <branch>
```

