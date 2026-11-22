# 21. Inspect branch upstream configuration

Understand which remote branch status and pull commands refer to.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git branch -vv
git rev-parse --abbrev-ref --symbolic-full-name '@{upstream}'
```

An upstream is branch configuration, not a live connection. The rev-parse command fails when no upstream exists. Quote @{upstream} in PowerShell so the shell does not interpret its braces.

## Exercise

On a scratch topic branch, compare its upstream with main's. Set an upstream only after confirming the intended remote destination.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-branch)

[Return to the lab index](../README.md)
