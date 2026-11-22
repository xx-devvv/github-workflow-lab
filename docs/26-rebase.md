# 26. Replay a private topic branch onto an updated base

Understand how rebasing changes commit identities while preserving intended edits.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git switch practice/topic
git fetch origin
git rebase origin/main
git log --oneline --decorate -6
```

Rebase normally creates new commits and may stop on conflicts. Use it on a private scratch branch. Rewriting a branch others use requires coordination; do not force-push as an automatic follow-up.

## Exercise

If stopped, inspect git status. Use git rebase --continue after resolving and staging, or git rebase --abort to abandon an in-progress attempt.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-rebase)

[Return to the lab index](../README.md)
