# Basic Git Commands

## Initialize repository
```bash
git init

Check repository status
git status

Stage changes
git add .

Commit changes
git commit -m "Meaningful commit message"

View commit history
git log --oneline

---

## 3️⃣ `branching.md`

```md
# Branching Basics

Branches allow working on features without affecting the main codebase.

## Create a new branch
```bash
git branch feature-login

Switch to a branch
git checkout feature-login

Create and switch (shortcut)
git checkout -b feature-login

Merge a branch
git checkout main
git merge feature-login


---

## 4️⃣ `commit-messages.md`

```md
# Commit Messages

Good commit messages make project history readable and useful.

## Good examples
- Add initial project structure
- Fix typo in README
- Update Docker configuration

## Bad examples
- update
- fix
- changes

## Simple rule
Each commit should describe **what** was changed, not **how**.
