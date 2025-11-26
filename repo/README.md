# Day 7 Repo — Git Basics

This folder is your local Git playground for AutoOps+ Day 7. :contentReference[oaicite:4]{index=4}  

## Tasks

1. Initialize Git:

   ```bash
   git init
   ```
2. Stage and commit all files:

   ```bash
   git add .
   git commit -m "feat: initial project structure"
   ```
3. Edit script.sh,run:
   ```bash
   git status
   git add script.sh
   git commit -m "feat: update script message"
   ```
4. View history:
   ```bash
   git log --oneline
   ```
5. Practice undo:
   ```bash
   git restore script.sh        # discard changes to script.sh
   git reset --soft -HEAD-1     # undo last commit but keep changes
   ```

