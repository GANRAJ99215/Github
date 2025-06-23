# 🧠 Git Commands: Basic to Advanced Cheat Sheet

This is a complete guide from basic to advanced Git commands with clear explanations.

---

## 📁 Repository Setup & Creating Projects

```
git init
```
---Create a new local Git repository

```
git clone <repo-url>
```
---Copy a remote repo to your local machine

```
git remote -v
```
---List connected remote repositories

```
git remote add origin <url>
```
---Connect your local repository to a remote

```
git init --bare
```
---Create a bare Git repository (remote only)

```
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```
---Set your Git identity globally

```
git config --list
```
---View all configured Git settings

```
git remote rename origin upstream
```
---Rename an existing remote

---

## 📝 Staging & Committing / Snapshotting

```
git status
```
---Show status of working directory and staged files

```
git add .
```
---Stage all modified and new files

```
git add <file>
```
---Stage a specific file

```
git add -A
```
---Stage all changes including deletions

```
git add -u
```
---Stage modified and deleted files

```
git commit -m "message"
```
---Commit staged changes with a message

```
git commit --amend
```
---Modify the most recent commit

```
git rm -r <file>
```
---Remove a file or folder

```
git clean -fd
```
---Remove untracked files and folders (force)

---

## 🌿 Branching & Merging

```
git branch
```
---List all local branches

```
git branch -a
```
---List all branches including remote

```
git branch <name>
```
---Create a new branch

```
git branch -d <name>
```
---Delete a branch

```
git branch -m <old> <new>
```
---Rename a local branch

```
git checkout -b <name>
```
---Create and switch to a new branch

```
git checkout <name>
```
---Switch to a branch

```
git merge <branch>
```
---Merge specified branch into current

```
git merge <source> <target>
```
---Merge source into target branch

```
git rebase <branch>
```
---Reapply commits on top of another branch

```
git cherry-pick <commit>
```
---Apply specific commit to current branch

```
git stash
```
---Stash current changes temporarily

```
git stash pop
```
---Apply and remove last stashed changes

```
git stash apply
```
---Apply last stash (without deleting)

```
git stash clear
```
---Delete all stashes

---

## 🚀 Pushing & Pulling / Collaboration

```
git push
```
---Push committed changes to remote

```
git push origin <branch>
```
---Push specific branch to remote

```
git push -u origin <branch>
```
---Push and set upstream branch

```
git push origin --delete <branch>
```
---Delete a branch from remote

```
git pull
```
---Download and merge from remote

```
git pull origin <branch>
```
---Pull specific branch from remote

```
git pull --rebase
```
---Pull with rebase instead of merge

```
git fetch
```
---Download changes from remote without merging

```
git fetch --prune
```
---Fetch and clean up removed branches

---

## 🧾 Logs and History

```
git log
```
---View commit history

```
git log --oneline
```
---Condensed one-line history

```
git log --oneline --graph
```
---Graphical view of history

```
git show <commit>
```
---Show details of a commit

```
git log --summary
```
---Detailed commit changes

```
git diff
```
---Compare working directory and index

```
git diff --cached
```
---Compare staged changes and last commit

```
git diff <source> <target>
```
---Preview differences between branches

```
git blame <file>
```
---Show who last modified each line

```
git shortlog
```
---Summary of commits by user

```
git reflog
```
---History of branch and HEAD changes

---

## ⏪ Resetting & Reverting

```
git reset --hard <commit>
```
---Reset history and discard all changes

```
git revert <commit>
```
---Create a new commit to undo a specific commit

```
git checkout -- <file>
```
---Discard changes to a file

---

## 🔖 Tagging & Releases

```
git tag
```
---List all tags

```
git tag <tag>
```
---Create a simple tag

```
git tag -a <tag> -m "message"
```
---Create an annotated tag

```
git push origin <tag>
```
---Push a tag to remote

```
git tag -d <tag>
```
---Delete a local tag

```
git push origin :refs/tags/<tag>
```
---Delete a tag on remote

```
git describe --tags
```
---Show latest tag relative to current commit

---

## 📦 Miscellaneous & Tools

```
git archive -o latest.zip HEAD
```
---Export repository as zip

```
git grep <pattern>
```
---Search for a pattern in tracked files

```
git bisect start
git bisect bad
git bisect good <commit>
```
---Find the commit that introduced a bug
