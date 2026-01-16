# TASK 2: Git & GitHub Fundamentals

## 📝 Objective
This repository demonstrates the complete workflow of **Git and GitHub fundamentals**, including version control, branching, merging, rollback, and collaboration.  

The goal is to provide a **real-world DevOps workflow** experience.

---

## 🛠️ Tools Used
- **Primary:** Git, GitHub  
- **Alternatives:** GitLab, Bitbucket  

---

## 1️⃣ Install Git & Configure User

### 🔹 Install Git
```bash
sudo apt update
sudo apt install git -y
```
---
### 🔹 Configure Git globally
```
git config --global user.name "Manohar R"
git config --global user.email "your-email@example.com"
```
---
### 🔹 Verify configuration
```
git config --list
```
---
## 2️⃣ Initialize Local Git Repository

### 🔹 Create project directory
```
mkdir git-task-2
cd git-task-2
```
---
### 🔹 Initialize Git
```
git init
```
Creates a hidden .git/ directory to track changes and commits.
---
## 3️⃣ Create Files & Commit Changes

### 🔹 Create a file
```
nano README.md
```
Add:
# Git & GitHub Fundamentals
This repository is created as part of Task 2.
---
### 🔹 Stage and commit
```
git add README.md
git commit -m "Initial commit: added README"
```
---
## 4️⃣ Create GitHub Repository & Link Local Repo

Create a new GitHub repository: task2-git-github-fundamentals

Add remote:
```
git remote add origin https://github.com/<username>/task2-git-github-fundamentals.git
git remote -v
```
## 5️⃣ Push Local Commits to GitHub
```
git branch -M main
git push -u origin main
```
✅ Now your code is on GitHub.
---
## 6️⃣ Branching & Merging
### 🔹 Create a feature branch
```
git checkout -b feature-update
```
### 🔹 Make changes and commit
```
echo "Branching practice" >> README.md
git add .
git commit -m "Updated README from feature branch"
```
### 🔹 Merge branch back into main
```
git checkout main
git merge feature-update
```
---
## 7️⃣ Rollback & Undo Changes

### 🔹 View commit history
```
git log --oneline
```
### 🔹 Reset to previous commit (local)
```
git reset --hard <commit-id>
```
### 🔹 Undo commit in shared repo safely
```
git revert <commit-id>
```
---
## 8️⃣ Common Git Commands Used
| Command                   | Purpose                            |
| ------------------------- | ---------------------------------- |
| `git status`              | Check file and commit status       |
| `git add <file>`          | Stage files for commit             |
| `git commit -m "message"` | Commit staged changes              |
| `git log`                 | View commit history                |
| `git branch`              | List or create branches            |
| `git checkout`            | Switch branches or commits         |
| `git merge`               | Merge branches                     |
| `git reset`               | Undo commits locally               |
| `git revert`              | Undo commits safely in shared repo |

---
## 9️⃣ Deliverables

GitHub repository link:
https://github.com/<username>/task2-git-github-fundamentals

Commit history screenshots

Branch creation & merge screenshots

Rollback practice evidence

---
## ✅ Outcome

Complete real-world Git workflow experience

Hands-on practice with branching, merging, rollback

Ready for DevOps interviews
