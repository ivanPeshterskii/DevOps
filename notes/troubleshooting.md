# Troubleshooting

## Quick tip
When stuck, run `git status` first.

## Git pull: divergent branches
**Issue:** `fatal: Need to specify how to reconcile divergent branches.`  
**Cause:** Local and remote branches had different commits.  
**Fix:** Use merge pull:
```bash
git pull --no-rebase origin main

Optional default:
git config pull.rebase false

Docker: Cannot connect to the Docker daemon
Issue: Cannot connect to the Docker daemon at ... docker.sock
Cause: Docker Desktop (Engine) was not running.
Fix: Start Docker Desktop and verify:
docker info


---

## 4) `notes/interview-notes.md`

```md
# Interview Notes

## How to explain Docker (simple)
Docker packages an app and everything it needs to run into a container,
so it works the same way across different machines.

## What my CI does
On every push to `main`, GitHub Actions checks out the repository and builds
the Docker image. If the build fails, the pipeline fails.

## What I want to learn next
- multi-stage Docker builds
- basic Kubernetes concepts
- deployment strategies