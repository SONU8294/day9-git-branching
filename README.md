# Day 9 – Git Branching & Merging (DevOps Learning Plan)

This project covers **Git branching, merging, conflict resolution**, and pushing multiple branches to GitHub. These concepts are essential for DevOps, CI/CD pipelines, and collaborative development.

---

## 🔥 Topics Covered

### ✅ Initialize Git Repository  
- Created folder `day9_git_branching`
- Initialized Git repo using `git init`
- Created initial file: `app.txt`

### ✅ Created Multiple Branches
- `feature-login`
- `feature-logout`

Commands used:
```bash
git branch feature-login
git branch feature-logout
git checkout feature-login
git checkout feature-logout


✨ Work Done in Each Branch
🔹 feature-login Branch

Added login feature:

echo "Login feature code here" > app.txt

🔹 feature-logout Branch

Added logout feature:

echo "Logout feature code here" >> app.txt

🔀 Merging Branches
1️⃣ Merge feature-login into master
git checkout master
git merge feature-login

2️⃣ Merge feature-logout into master

This created a merge conflict in app.txt.

Conflict example:

<<<<<<< HEAD
Login feature code here
=======
Logout feature code here
>>>>>>> feature-logout

🛠 Conflict Resolved By:

Manually updating the file to:

Login feature code here
Logout feature code here


Then:

git add app.txt
git commit -m "Resolved merge conflict"

📤 Pushed to GitHub

Repository URL:

➡️ https://github.com/SONU8294/day9-git-branching

Pushed master branch:

git push -u origin master

🎯 Learning Outcome

By completing Day 9 you learned:

How to create Git branches

Switching between branches

Adding new changes per branch

Merging branches

Handling merge conflicts

Pushing your local repo to GitHub
