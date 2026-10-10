# Proof of Work - fax9

**Repository:** https://github.com/fax9/devops-git-challenge

## Commit History (git log --oneline)
```
bfcd596 fix: remove blank line before shebang
a50b6e5 Merge pull request #1 from fax9/development
c9f747c fix: resolved merge conflict
b1664b7 fix: staging label
8cc7d00 feat: updated script with staging env
3424f91 feat: initial commit with deploy script
4aa7fcc Initial commit
```

## Reflection Questions

### Q1: Difference between Git (local tracking) and GitHub (cloud platform)
Git is software installed on your computer that tracks file versions locally and works offline.
GitHub is a website that hosts Git repositories online so they can be backed up, shared, and worked on by a team. 
It adds features like pull requests, issues, and access control.
In this lab, for example, you committed with Git locally and then merged the PR on GitHub.

### Q2: Working Directory, Staging Area, and Local Repository
The working directory is where you actually edit files, like when you edited deploy.sh in nano.
The staging area holds changes you’ve chosen with git add to go into the next commit.
The local repository (the .git folder) stores the permanent snapshots created by git commit.

### Q3: Difference between git stash pop and git stash apply
Both bring back stashed changes. pop applies them and then deletes the stash;
your terminal showed “Dropped refs/stash@{0}” when you did this.
apply restores the changes but keeps the stash in the list, so you could reuse it on another branch.

### Q4: Difference between git fetch and git pull
git fetch downloads new commits from GitHub but doesn’t change your files or branch, 
so you can inspect them first. git pull does a fetch and then immediately merges the changes
into your current branch, which is what you did after merging the PR.
