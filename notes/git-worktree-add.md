# Git: a second working directory with worktree

`git worktree` checks out another branch in a separate directory that shares the same repository, so you can handle a hotfix without stashing.

```bash
git worktree add ../hotfix -b hotfix/123 origin/main
```
