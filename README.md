# AutoOps+ Day 7 — Git Basics (Local Operations)

This repository contains hands-on exercises for local Git workflows:

- `git init`
- `git add`
- `git commit`
- `git status`
- `git log`
- basic undo commands (`git restore`, `git reset`)

It aligns with Domain 1.2 of the CompTIA AutoOps+ objectives. :contentReference[oaicite:2]{index=2}  

## 📁 Folder Structure
```
autoops-day7-git-basics/
│
├── README.md
│
├── repo/
│   ├── script.sh
│   ├── README.md
│   └── notes.md
│
└── exercises/
    ├── exercise1.txt
    └── exercise2.txt
```

## 🧩 Repo Layout

- `repo/` — where you actually practice Git (init, add, commit, log, undo)
- `exercises/` — simple prompts to guide your commits

-

## 🚀 Getting Started

From the root of this project:

```bash
cd repo
git init
```

Configure your identity (only once per machine):
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Check status:
```bash
git status
```

## 📝 Stage and Commit Files

Stage all files:
```bash
git add .
```

Create your first commit:
```bash
git commit -m "feat: initial commit"
```

Make a change in script.sh or notes.md, then:
```bash
git status
git add script.sh
git commit -m "feat: add basic script output"
```

View history:
```bash
git log --oneline
```

## ↩️ Undo Examples

Unstage a file:
```bash
git restore --staged script.sh
```

Discard local changes in a file:
```bash
git restore script.sh
```

Undo the last commit but keep the changes:
```bash
git reset --soft HEAD-1
```

Hard reset (dangerous, loses changes):
```bash
git reset --hard HEAD-1
```

## 🎯 Goals for Day 7

-Understand working directory → staging area → repository

-Create clean, meaningful commit messages

-View and interpret commit history

-Practice fixing mistakes with restore and reset

-Prepare for AutoOps+ Domain 1.2 (source control)

Happy commiting!

NOTE: (Make script.sh executible if you want to run it:)
```bash
chmod +x repo/script.sh
./repo/script.sh
```
