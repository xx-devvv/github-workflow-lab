# 20. Choose a predictable pull policy

Integrate remote changes only when a fast-forward is possible.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git status --short
git branch --show-current
git pull --ff-only origin main
```

Run this on the local main branch with a clean working tree. --ff-only refuses divergent history. It is useful for a default branch that should follow the remote without creating accidental merge commits.

## Exercise

If the command refuses, inspect the divergence first. Decide how to preserve local work before choosing merge or rebase.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-pull)

[Return to the lab index](../README.md)
