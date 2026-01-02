# Branching in Git

Branching allows developers to work on features, fixes, or experiments
without affecting the main codebase.

It is a core concept in collaborative development.

---

## What is a branch?

A branch is a pointer to a specific commit.
The default branch is usually called `main`.

Branches make it possible to:
- develop features in isolation
- fix bugs safely
- keep `main` stable

---

## Create a new branch

```bash
git branch feature-git-notes

Switch to a branch
git checkout feature-git-notes

Create and switch in one command
git checkout -b feature-git-notes

Check existing branches
git branch

The current branch is marked with *.

Merge a branch into main
git checkout main
git merge feature-git-notes
This combines the work from the feature branch into main.

Delete a branch (after merge)
git branch -d feature-git-notes

## Good practices
Keep branches small and focused
Name branches clearly (feature-, fix-, hotfix-)
Delete branches after merging