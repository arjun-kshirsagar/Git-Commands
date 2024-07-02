# Essential Git Commands

## Introduction
This repository contains a curated list of essential Git commands, organized by functionality. It serves as a quick reference guide for developers to improve their version control workflow.

## Table of Contents
1. [Repository Setup](#repository-setup)
2. [Branching](#branching)
3. [Committing](#committing)
4. [Staging](#staging)
5. [Merging](#merging)
6. [Remote Repositories](#remote-repositories)
7. [Stashing and Cleaning](#stashing-and-cleaning)
8. [Rebasing](#rebasing)
9. [Undoing Changes](#undoing-changes)
10. [Viewing History](#viewing-history)

## Repository Setup
Initialize a new Git repository:
  ```
  git init 
  ```

Clone an existing repository:
```
git clone <repository_url>
```
To deactivate a GitHub repository on your desktop, you can simply remove the .git directory from your local repository. This effectively "deactivates" Git in that directory.
```
rm -rf .git
```

## Branching

List all branches:
``` 
git branch
```
Create a new branch:
```
git branch <branch_name>
```
Switch to a branch:
```
git checkout <branch_name>
```
Create and switch to a new branch:
```
git checkout -b <branch_name>
```
Merge a branch into the current branch:
```
git merge <branch_name>
```

## Committing
Add changes to the staging area:
```
git add <file_or_directory>
```
Commit changes:
```
git commit -m "commit message"
```
Add and commit changes:
```
git commit -am "commit message"
```

## Staging
View staged and unstaged changes:
```
git status
```

## Merging
Merge a branch into the current branch:
```
git merge <branch_name>
```

## Remote Repositories
Add a remote repository:
```
git remote add origin <repository_url>
```
Push changes to the remote repository:
```
git push origin <branch_name>
```
Pull changes from the remote repository:
```
git pull origin <branch_name>
```

## Stashing and Cleaning
Stash changes:
```
git stash
```
Apply stashed changes:
```
git stash apply
```
Clean untracked files:
```
git clean -f
```

## Rebasing
Rebase current branch onto another branch:
```
git rebase <branch_name>
```

## Undoing Changes
Undo the last commit (keep changes):
```
git reset --soft HEAD~1
```

Undo the last commit (discard changes):
```
git reset --hard HEAD~1
```

## Viewing History
View commit history:
``` 
git log 
```

View commit history with graphical representation:
```
git log --graph --oneline --all
```
