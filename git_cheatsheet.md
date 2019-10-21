# Git Commands List
git [add](#git-add) |
git [clone](#git-clone) |
git [config](#git-config) |
git [fetch](#git-fetch) |
git [init](#git-init) |
git [pull](#git-pull) |
git [push](#git-push) |
git [remote](#git-remote) |

# Git Commands

## Git Basics
Create empty Git repo in specified directory. 

### git init
Run with no arguments to initialize the current directory as a git repository
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

Devs commonly use --global flag to set config options for current user.
```bash
git config user.name <name>
```

### git add
Stage all changes in <directory> / <file> for the next commit.
  
Replace <directory> with a <file> to change a specific file.
```bash
git add <directory>
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

