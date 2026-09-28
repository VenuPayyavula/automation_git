# 🎮 GitQuest — Your Interactive Git Learning Guide
## Player: Venu Payyavula | Project: Automation Classes

---

# 🗺️ THE QUEST MAP

```
🏠 START → ⚔️ L1: What is Git? → 🔧 L2: Setup → 📦 L3: Repository
→ 💾 L4: Stage & Commit → 🌿 L5: Branching → ☁️ L6: Remote
→ 🔍 L7: PR & Review → 🏆 L8: Real Workflow → 👑 GIT MASTER
```

---

# ✅ LEVEL 1 — What is Git? [COMPLETED 🏆]

Git is a **Version Control System (VCS)** — it tracks every change to your code like a time machine.

### The 4 Zones of Git:
| Zone | What it is | Analogy |
|------|-----------|---------|
| Working Directory | Your files on disk | Your desk |
| Staging Area | Files ready to save | Envelope before posting |
| Local Repository | Saved history on your PC | Personal diary |
| Remote Repository | Cloud backup + team share | Google Drive for teams |

---

# ✅ LEVEL 2 — Setup & Configuration [COMPLETED 🏆]

### Your Identity is Set:
- **Name:** VenuPayyavula
- **Email:** bunnyvenu7172@gmail.com
- **Default Branch:** master

### Key Commands Learned:
| Command | What it does |
|---------|-------------|
| `git --version` | Check if Git is installed |
| `git config --global user.name "Your Name"` | Set your name |
| `git config --global user.email "email"` | Set your email |
| `git config --list` | See all settings |

### 💡 Pro Tip — Pager Exit:
When Git shows `(END)` in terminal → Press **`q`** to quit!
To avoid pager always, use flag: `--no-pager`

---

# 🔄 LEVEL 3 — Your Repository [IN PROGRESS ⚔️]

## What is a Repository?

A **Repository (Repo)** is Git's database for your project.
Think of it as a **save-file folder** that tracks ALL history of your project.

```
📁 Automation classes/          ← Your project folder
├── 📂 .git/                    ← 🔒 Git's secret database (DON'T TOUCH!)
│   ├── config                  ← repo settings
│   ├── HEAD                    ← which branch you're on
│   └── objects/                ← all your saved snapshots
├── 📂 tests/
│   ├── AdminPage.spec.ts
│   ├── PIM.spec.ts
│   ├── Leave.spec.ts
│   └── example.spec.ts
├── .gitignore                  ← files Git should ignore
├── package.json
└── playwright.config.ts
```

## Key Commands for Level 3:

| Command | What it does | When to use |
|---------|-------------|-------------|
| `git init` | Create a new repo in current folder | Starting fresh |
| `git status` | See what's changed / what's new | ALWAYS — before anything |
| `git log --oneline` | See history of commits (save points) | To review past saves |
| `git --no-pager log --oneline` | Same but no scroll view | Cleaner output |
| `git remote -v` | See connected remote (GitHub) servers | Check cloud connections |

## 🎯 Why `git --no-pager log --oneline`?

Breaking it down:
- `git` → the git program
- `--no-pager` → don't open scroll viewer (no `(END)` prompt!)
- `log` → show history of commits
- `--oneline` → show each commit in ONE line (compact view)

**Output looks like:**
```
a3f9c2b Add Leave page tests
9d1e7f3 Add PIM module tests
c48b2a1 Initial project setup
```
Each line = one save point (commit) with its ID and message.

---

# 💾 LEVEL 4 — Staging & Committing [COMING SOON]

## The 3-Step Save Process:
```
1. MODIFY files    →  git status     (see what changed)
2. STAGE files     →  git add        (pick what to save)
3. COMMIT          →  git commit -m  (actually save it)
```

### Key Commands:
| Command | What it does |
|---------|-------------|
| `git status` | See all changed/new files |
| `git add filename` | Stage ONE specific file |
| `git add .` | Stage ALL changed files |
| `git commit -m "message"` | Save staged files with a message |
| `git diff` | See exactly what lines changed |

---

# 🌿 LEVEL 5 — Branching [COMING SOON]

Branches = **Parallel universes** for your code.
- `main/master` = The stable production universe
- `feature/login-tests` = Your experimental universe

### Key Commands:
| Command | What it does |
|---------|-------------|
| `git branch` | List all branches |
| `git branch feature-name` | Create new branch |
| `git checkout branch-name` | Switch to branch |
| `git checkout -b feature-name` | Create AND switch in one step |
| `git merge branch-name` | Merge branch into current |

---

# ☁️ LEVEL 6 — Remote Repository [COMING SOON]

### Key Commands:
| Command | What it does |
|---------|-------------|
| `git remote add origin URL` | Connect to GitHub repo |
| `git push origin main` | Upload local → GitHub |
| `git pull origin main` | Download GitHub → local |
| `git clone URL` | Download entire repo from GitHub |
| `git fetch` | Check for remote changes (no merge) |

---

# 🔍 LEVEL 7 — Pull Requests & Code Review [COMING SOON]

### Your Two Roles:
| Role | Account | Actions |
|------|---------|---------|
| 👷 Contributor | Primary account | Create branch → Push → Raise PR |
| 🔍 Reviewer | Second account | Review PR → Approve → Merge |

---

# 🏆 LEVEL 8 — Real Automation Workflow [COMING SOON]

Full real-world Git workflow applied to your Playwright test project!

---

# 📖 QUICK REFERENCE CHEAT SHEET

## Most Used Commands (Daily):
```bash
git status                    # What's changed? (USE THIS ALWAYS FIRST)
git add .                     # Stage all changes
git commit -m "your message"  # Save with description
git push origin branch-name   # Upload to GitHub
git pull origin main          # Get latest from GitHub
git branch                    # Which branch am I on?
git log --oneline             # See commit history
```

## The Golden Git Workflow:
```
Pull latest → Create branch → Make changes → 
Stage → Commit → Push → Create PR → Review → Merge
```

---

*Last Updated: Level 3 in progress*
