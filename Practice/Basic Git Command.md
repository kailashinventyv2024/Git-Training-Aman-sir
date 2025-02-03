## Basic Git Commands Cheat Sheet
### Setup & Configuration

``` bash
git config --global user.name "Kailash8799"
git config --global user.email "kailash@gmail.com"
```

### Initialize a Repository
```bash
git init
```

###  Clone a Repository
```bash
git clone https://github.com/kailash8799/ClipX.git
```

### Add a Remote
```bash
git remote add origin https://github.com/kailash8799/ClipX.git
```

### List Remotes
```bash
git remote -v
```

## Basic Workflow

### Check Status
```bash
git status
```

###  Stage Changes
```bash
git add filename  # Stage specific file
git add . # Stage all changes
git add -A  # Stage all (new/modified/deleted)
```

### Commit Changes
```bash
git commit -m "my message"
```

### Unstage a File
```bash 
git reset HEAD filename
```

## Branching & Merging
### Create a New Branch
```bash
git branch new-branch
```

### Switch Branches
```bash
git checkout feature1
git checkout -b feature1  # Create and switch to new branch
```

### Merge Branches
```bash
git checkout main # Switch to target branch
git merge feature1   # Merge feature1 into main
```

### Delete a Branch
```bash
git branch -d feature1   # Delete locally
git push origin --delete feature1  # Delete remote branch
```

## Syncing with Remote
### Fetch Changes
```bash
git fetch origin  # Fetch updates without merging
```
### Pull Updates
```bash
git pull origin main   # Fetch + merge (equivalent to fetch + merge)
```

### Push Changes
```bash
git push origin main # Push local commits to remote
```

## Viewing History
### View Commit Log
```bash
git log # Show full history
git log --oneline --graph # Compact view with branch visualization
```

### Compare Changes
```bash
git diff  # Show unstaged changes
git diff --staged  # Show staged changes
```