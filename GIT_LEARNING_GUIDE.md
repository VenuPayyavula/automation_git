# 🎮 GitQuest — Your Interactive Git Learning Guide
## Player: Venu Payyavula | Project: Automation Classes
## Status: GIT MASTER 👑

---

# 🗺️ THE QUEST MAP — ALL LEVELS COMPLETE!

```
✅ L1: What is Git?  →  ✅ L2: Setup  →  ✅ L3: Repository
✅ L4: Stage & Commit  →  ✅ L5: Branching  →  ✅ L6: Remote
✅ L7: Pull Requests  →  ✅ L8: Real Workflow  →  👑 GIT MASTER
```

---

# ⚡ DAILY CHEAT SHEET (Use This Every Day!)

## 🌅 Start of Day:
```bash
git checkout master          # Go to master branch
git pull                     # Get latest from GitHub
git checkout -b feature/task-name  # Create your branch
```

## 💻 During Work:
```bash
git status                   # What changed? (run this often!)
git diff filename            # See exact line changes
git add .                    # Stage all changes
git add filename             # Stage one specific file
git commit -m "feat: message" # Save with meaningful message
```

## ☁️ Pushing & PR:
```bash
git push -u origin feature/task-name  # First push of branch
git push                     # Subsequent pushes (after -u is set)
```
Then go to GitHub → Create Pull Request → Get Review → Merge

## 🧹 End of Task Cleanup:
```bash
git checkout master          # Switch back to master
git pull                     # Sync merged changes
git branch -d feature/task-name  # Delete merged branch
```

---

# 📖 COMPLETE REFERENCE

## ✅ LEVEL 1 — What is Git? [MASTERED 🏆]

Git is a **Version Control System (VCS)** — tracks every change to your code like a time machine.

### The 4 Zones of Git:
| Zone | What it is | Analogy |
|------|-----------|---------|
| Working Directory | Your files on disk | Your desk |
| Staging Area | Files ready to save | Envelope before posting |
| Local Repository | Saved history on your PC | Personal diary |
| Remote Repository | Cloud backup + team share | Google Drive for teams |

---

## ✅ LEVEL 2 — Setup & Configuration [MASTERED 🏆]

### Your Identity:
- **Name:** VenuPayyavula
- **Email:** bunnyvenu7172@gmail.com
- **Remote Repo:** https://github.com/VenuPayyavula/automation_git.git

### Key Commands:
| Command | What it does |
|---------|-------------|
| `git --version` | Check if Git is installed |
| `git config --global user.name "Name"` | Set your name |
| `git config --global user.email "email"` | Set your email |
| `git config --list` | See all settings |

### 💡 Pro Tips:
- When Git shows `(END)` → Press **`q`** to quit
- `2>&1` = redirect error output to terminal (you don't need to type this yourself)
- `&&` = "AND THEN" — run next command only if previous succeeded

---

## ✅ LEVEL 3 — Your Repository [MASTERED 🏆]

### Key Commands:
| Command | 🎯 Purpose |
|---------|-----------|
| `git init` | Create new repo in current folder |
| `git status` | See what's changed / untracked / staged |
| `git log --oneline` | See compact commit history |
| `git log --oneline --graph --all` | Visual branch tree |
| `git remote -v` | See connected GitHub servers |

### 📁 Your Project Structure:
```
📁 Automation classes/
├── 📂 .git/            ← Git's secret database (DON'T TOUCH!)
├── 📂 tests/
│   ├── AdminPage.spec.ts
│   ├── PIM.spec.ts
│   ├── Leave.spec.ts
│   ├── DashboardPage.spec.ts
│   └── example.spec.ts
├── .gitignore
├── GIT_LEARNING_GUIDE.md
├── package.json
└── playwright.config.ts
```

---

## ✅ LEVEL 4 — Staging & Committing [MASTERED 🏆]

### The 3 States of Every File:
| State | Color in git status | How to move forward |
|-------|---------------------|---------------------|
| 🔴 Untracked | Red | `git add filename` |
| 🟡 Modified | Red | `git add filename` |
| 🟢 Staged | Green | `git commit -m "message"` |
| ✅ Committed | Clean | `git push` |

### Key Commands:
| Command | 🎯 Purpose |
|---------|-----------|
| `git status` | See all file states |
| `git add filename` | Stage ONE file |
| `git add .` | Stage ALL changed files |
| `git diff filename` | See exact line changes |
| `git commit -m "message"` | Save staged files |
| `git restore filename` | Discard unstaged changes |
| `git restore --staged filename` | Unstage a file |

### ✅ Good Commit Messages:
```
feat: add AdminPage login test cases
fix: PIM search returning wrong results  
test: add Leave module edge case tests
chore: update playwright config timeout
docs: add test execution README
refactor: extract reusable login helper
```

### ❌ Bad Commit Messages:
```
changes / stuff / fix / update / asdfgh
```

---

## ✅ LEVEL 5 — Branching [MASTERED 🏆]

### Branch Naming Conventions:
| Pattern | Example |
|---------|---------|
| `feature/description` | `feature/admin-login-tests` |
| `fix/description` | `fix/pim-null-error` |
| `hotfix/description` | `hotfix/login-crash` |
| `your-name/task` | `venu/dashboard-tests` |

### Key Commands:
| Command | 🎯 Purpose |
|---------|-----------|
| `git branch` | List all branches (* = current) |
| `git checkout -b branch-name` | Create AND switch to new branch |
| `git checkout branch-name` | Switch to existing branch |
| `git merge branch-name` | Bring another branch into current |
| `git branch -d branch-name` | Delete a merged branch |

### 🏷️ Branch Golden Rules:
- ✅ Always create branch FROM master
- ✅ Work ONLY on your own branch
- ✅ Push branch to GitHub before PR
- ✅ Delete branch after merge
- ❌ NEVER commit directly to master in a team

### HEAD Explained:
- `HEAD` = "You Are Here" marker in Git history
- `HEAD -> master` = You're on master branch
- `HEAD -> feature/x` = You're on feature/x branch

---

## ✅ LEVEL 6 — Remote Repositories [MASTERED 🏆]

### Key Commands:
| Command | 🎯 Purpose |
|---------|-----------|
| `git remote add origin URL` | Connect local repo to GitHub |
| `git remote -v` | Verify remote connection |
| `git push -u origin master` | Upload + set tracking (first time) |
| `git push` | Upload (after -u is set) |
| `git pull` | Download + merge from GitHub |
| `git fetch` | Download but don't merge |
| `git clone URL` | Download entire repo from GitHub |

### 💡 Key Concepts:
- `origin` = nickname for your GitHub remote URL
- `-u` flag = sets tracking so future `git push` needs no extra args
- `git pull` = `git fetch` + `git merge` in one command
- Windows Git Credential Manager handles authentication via browser

---

## ✅ LEVEL 7 — Pull Requests & Code Review [MASTERED 🏆]

### What is a PR?
A Pull Request = formal request to merge your branch into master AFTER review.

### The PR Flow:
```
feature branch → push → GitHub PR → Review → Approve → Merge → master
```

### Reviewer Actions on GitHub:
| Action | Meaning |
|--------|---------|
| **Comment** | General feedback, no approval |
| **Approve** | Code is good, ready to merge |
| **Request changes** | Fix these issues first |
| **Merge** | Bring branch into master (repo owner) |

### Files Changed Tab:
- 🟩 Green lines with `+` = Lines ADDED
- 🟥 Red lines with `-` = Lines REMOVED
- `@@ -0,0 +1 @@` = Diff header (lines before → lines after)

### GitHub Security Rule:
- You CANNOT approve your OWN PR (requires second reviewer)
- But repo OWNER can always merge directly

### PR Best Practices:
- One PR = One feature/fix (keep it small!)
- Write a clear description of what changed and why
- Respond to reviewer comments before merging
- Delete branch after merge (GitHub prompts you!)

---

## ✅ LEVEL 8 — Real Daily Workflow [MASTERED 🏆]

### Your Complete Daily Git Ritual:

#### 🌅 MORNING — Sync Up:
```bash
git checkout master
git pull
```

#### 🌿 START TASK — Create Branch:
```bash
git checkout -b feature/task-description
git branch   # verify you're on new branch
git status   # verify clean state
```

#### 💻 DURING WORK — Save Progress Often:
```bash
git status              # see what changed
git diff tests/file.ts  # see exact changes
git add .               # stage all
git commit -m "feat: description of what you did"
# Repeat: work → add → commit (multiple times per day!)
```

#### ☁️ READY FOR REVIEW — Push & PR:
```bash
git push -u origin feature/task-description
# Go to GitHub → yellow banner → Create pull request
# Fill title + description → Create pull request
# Request review from teammate
```

#### ✅ AFTER MERGE — Clean Up:
```bash
git checkout master
git pull                              # get the merged changes
git branch -d feature/task-description  # delete local branch
git log --oneline                    # verify history
```

---

## 🚀 ADVANCED COMMANDS (Coming Soon!)

| Command | Purpose |
|---------|---------|
| `git stash` | Temporarily hide uncommitted changes |
| `git stash pop` | Bring back stashed changes |
| `git revert COMMIT_ID` | Undo a commit safely |
| `git reset --soft HEAD~1` | Undo last commit (keep changes staged) |
| `git cherry-pick COMMIT_ID` | Apply one specific commit to current branch |
| `git rebase master` | Update branch with latest master changes |

---

## 🏆 ACHIEVEMENTS UNLOCKED

| Badge | Level | Achievement |
|-------|-------|-------------|
| 🌱 "The Awakening" | L1 | Understood why Git exists |
| ⚙️ "Configured" | L2 | Set up Git identity |
| 📦 "Repository Born" | L3 | First repo initialized |
| 💾 "First Blood" | L4 | First commit ever! |
| 🌿 "Multiverse Explorer" | L5 | Proved branch isolation |
| 🌿 "Branch Master" | L5 | Full branch lifecycle complete |
| ☁️ "Cloud Warrior" | L6 | Code pushed to GitHub |
| 🔍 "The Gatekeeper" | L7 | Full PR cycle completed |
| 👑 "Git Master" | L8 | Real workflow mastered! |

---

*Completed: All 8 Levels | Repository: https://github.com/VenuPayyavula/automation_git*
