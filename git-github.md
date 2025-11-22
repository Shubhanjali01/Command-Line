

# 🟢 **1. Git Setup**

```
git init                    # Initialize a new Git repository
git clone <url>             # Clone a remote repository
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --list           # Show all git config settings
```

---

# 🔵 **2. Basic Snapshotting**

```
git status                  # Show changes
git add <file>              # Add a file
git add .                   # Add all files
git reset <file>            # Unstage a file
git reset                   # Unstage everything
git rm <file>               # Remove a file
git mv <old> <new>          # Rename a file
```

---

# 🟣 **3. Commit Commands**

```
git commit -m "message"             # Commit
git commit -am "message"            # Add + Commit tracked files
git commit --amend                  # Modify last commit
```

---

# 🔶 **4. Branch Commands**

```
git branch                          # List branches
git branch <name>                   # Create branch
git checkout <name>                 # Switch branch
git switch <name>                   # New way to switch
git switch -c <name>                # Create + switch
git merge <branch>                  # Merge branch
git branch -d <name>                # Delete branch
git branch -D <name>                # Force delete branch
```

---

# 🔷 **5. Remote Repository**

```
git remote -v                       # Show remotes
git remote add origin <url>         # Add remote
git remote remove origin            # Remove remote
git remote set-url origin <url>     # Change remote URL
```

---

# 🟡 **6. Push & Pull**

```
git push origin main                # Push to main
git push -u origin main             # Set upstream
git push                            # Push
git pull                            # Pull latest from remote
git fetch                           # Fetch updates only
git pull --rebase                   # Rebase pull
```

---

# 🔺 **7. Undoing Things**

```
git checkout -- <file>              # Undo file changes
git reset --hard                    # Reset everything
git reset --hard HEAD~1             # Delete last commit
git restore <file>                  # Restore changes
git revert <commit>                 # Create undo commit
```

---

# 🟤 **8. Viewing History**

```
git log                             # Full commit history
git log --oneline                   # One-line history
git log --graph                     # Branch graph
git show <commit>                   # Show details of a commit
git diff                            # Compare unstaged changes
git diff --staged                   # Compare staged changes
```

---

# ⚫ **9. Stash Commands**

```
git stash                           # Save work temporarily
git stash list                      # List stashes
git stash pop                       # Restore and delete stash
git stash apply                     # Restore without deleting
git stash drop                      # Remove a stash
```

---

# 🔘 **10. Tags**

```
git tag                             # List tags
git tag <tagname>                   # Create tag
git tag -a <tagname> -m "msg"       # Annotated tag
git push origin <tagname>           # Push tag
git push origin --tags              # Push all tags
```

---

# 🟠 **11. GitHub Authentication**

```
git config credential.helper store  # Store credentials
git credential-manager uninstall    # Remove manager
```

---

# 🟣 **12. Advanced Commands**

```
git cherry-pick <commit>            # Copy a commit to another branch
git rebase <branch>                 # Rebase
git reflog                          # Git history of HEAD
git bisect                          # Debug using binary search
git blame <file>                    # Show who changed each line
```

