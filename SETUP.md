# 🛠 SETUP GUIDE – Git + GitHub + Branch & PR Workflow

This guide explains **how to set up and use the repository** from scratch for beginners.

---

# 1️⃣ Install Git

### Windows

1. Download → [https://git-scm.com/downloads](https://git-scm.com/downloads)
2. Install with default options

### Mac

```bash
brew install git
```

### Linux

```bash
sudo apt update
sudo apt install git
```

### Verify Installation

```bash
git --version
```

---

# 2️⃣ First Time Git Configuration (Only Once)

```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@gmail.com"
```

Check configuration:

```bash
git config --list
```

---

# 3️⃣ Clone the Repository

Open terminal in the folder you want to store the repo:

```bash
git clone <repo-link>
cd DSA-Team-Practice
```

This will create the full folder structure locally.

---

# 4️⃣ Daily Workflow with Branches

## Step 1 – Pull Latest Main

Before starting work every day:

```bash
git pull origin main
```

## Step 2 – Create Your Branch

Each member works in their own branch:

```bash
git checkout -b yash-arrays
```

Branch naming convention: `<name>-<topic>`

## Step 3 – Add Your Code

Work **only inside your folder**:

```
Members/<YourName>/Questions/
Members/<YourName>/Solutions/
Members/<YourName>/Progress.md
```

Add code and save files.

## Step 4 – Stage & Commit Changes

```bash
git add .
git commit -m "add: two sum solution by yash"
```

## Step 5 – Push Branch

```bash
git push origin yash-arrays
```

---

# 5️⃣ Create Pull Request (PR)

1. Open GitHub → Repository → Pull Requests → New Pull Request
2. Select your branch → Submit PR
3. Add description: problem name, topic, difficulty, approach
4. Team reviews → Merge into main

> PR ensures main branch stays clean and reviewed.

---

# 6️⃣ Pull Latest Work (Daily)

```bash
git checkout main
git pull origin main
```

Always do this before starting new work.

---

# 7️⃣ Error Handling

## 1. Push Rejected

```bash
git pull origin main
git push origin <branch-name>
```

## 2. Undo All Changes

```bash
git restore .
```

## 3. Remove Last Commit

```bash
git reset --soft HEAD~1
```

## 4. Merge Conflict

Edit conflicted file, then:

```bash
git add .
git commit -m "resolve conflict"
git push origin <branch-name>
```

---

# 8️⃣ Golden Rules

✔ Work only inside your personal folder
✔ One problem = one file
✔ Include complexity and approach in each solution
✔ Pull main before pushing new changes
✔ Commit frequently with clear messages

---

# 9️⃣ Quick Command Summary

```bash
# Pull latest main
git checkout main
git pull origin main

# Create branch
git checkout -b <name-topic>

# Stage & commit
 git add .
git commit -m "message"

# Push branch
 git push origin <branch-name>

# After PR merge, update main
 git checkout main
git pull origin main
```

---

You are now ready to safely contribute using **branches + PR workflow**. Happy Coding 🚀
