# 🚀 Git Commands Reference Guide (DevOps / Production Level)

## 📌 Overview
Git is a distributed version control system used for:
- Source code management
- Team collaboration
- CI/CD pipelines
- Version tracking in DevOps workflows

---

All Git commands are laid out with the command on the left and its use/description on the right, grouped into 10 sections:

Setup & Config — username, email, list settings
Initialize & Clone — start repos locally or from remote
Staging & Committing — track and save changes
Branching — create, switch, delete branches
Merging & Rebasing — combine branches
Remote — push, pull, fetch from GitHub/GitLab etc.
Stash — temporarily shelve work
Log & History — explore commits and blame
Undoing Changes — restore, revert, reset
Tags — version tagging




# 🔐 0. Configuration

| Command | Description |
|--------|------------|
| `git config --global user.name "name"` | Sets global username |
| `git config --global user.email "email"` | Sets global email |
| `git config --list` | Displays all configuration settings |

---

# ⚙️ 1. Repository Setup

| Command | Description |
|--------|------------|
| `git --version` | Displays installed Git version |
| `git init` | Initializes a new Git repository |
| `git clone <repo-url>` | Clones an existing repository |

---

# 📂 2. Basic Workflow (Core Git Cycle)

| Command | Description |
|--------|------------|
| `git status` | Shows current working directory status |
| `git add <file>` | Stages specific file for commit |
| `git add .` | Stages all changes |
| `git commit -m "message"` | Commits staged changes |
| `git log` | Displays commit history |

---

# 🌿 3. Branching Strategy (Very Important in DevOps)

| Command | Description |
|--------|------------|
| `git branch` | Lists all local branches |
| `git branch <name>` | Creates a new branch |
| `git checkout <branch>` | Switches to a branch |
| `git checkout -b <branch>` | Creates and switches to new branch |
| `git merge <branch>` | Merges branch into current branch |
| `git branch -d <branch>` | Deletes a local branch |

---

# 🌐 4. Remote Repository Operations

| Command | Description |
|--------|------------|
| `git remote -v` | Shows remote repository URLs |
| `git remote add origin <url>` | Connects local repo to GitHub |
| `git push origin <branch>` | Pushes code to remote repository |
| `git pull origin <branch>` | Fetches and merges changes |
| `git fetch` | Fetches remote changes without merging |

---

# 🔄 5. Synchronization & Update Control

| Command | Description |
|--------|------------|
| `git pull` | Fetch + merge latest changes |
| `git fetch` | Downloads changes without merging |
| `git rebase` | Reapplies commits on top of another branch |

---

# 🧹 6. Undoing Changes (Critical for Production Safety)

| Command | Description |
|--------|------------|
| `git restore <file>` | Restores file to last committed state |
| `git reset <file>` | Unstages a file |
| `git reset --soft HEAD~1` | Undoes last commit (keeps changes) |
| `git reset --hard HEAD~1` | Completely removes last commit |
| `git revert <commit>` | Safely undoes a commit (creates new commit) |

---

# 📦 7. Stashing (Temporary Storage)

| Command | Description |
|--------|------------|
| `git stash` | Temporarily saves uncommitted changes |
| `git stash list` | Shows all stashes |
| `git stash pop` | Restores latest stash |
| `git stash drop` | Deletes stash |

---

# 🏷️ 8. Tagging (Release Management)

| Command | Description |
|--------|------------|
| `git tag` | Lists tags |
| `git tag <name>` | Creates a new tag |
| `git push origin <tag>` | Pushes tag to remote |

---



# 🔍 9. Inspection & Debugging

| Command | Description |
|--------|------------|
| `git diff` | Shows unstaged changes |
| `git diff --staged` | Shows staged changes |
| `git show <commit>` | Shows commit details |

---

