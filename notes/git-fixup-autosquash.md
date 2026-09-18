# Git: fixup commits with autosquash

Mark a commit as a fix for an earlier one and let rebase reorder it for you.

```bash
git commit --fixup <sha>
git rebase -i --autosquash <base>
```
