# 28. Find the common ancestor of two branches

Identify the shared starting point used in many comparisons.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git merge-base HEAD origin/main
git log --oneline --all --decorate --graph -12
git diff origin/main...HEAD --stat
```

A merge base is a best common ancestor. The three-dot diff compares the merge base with the right-hand revision; swapping sides changes what it shows. Complex histories can have more than one best merge base.

## Exercise

Use a branched scratch history to connect the reported ancestor with the graph and the three-dot diff.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-merge-base)

[Return to the lab index](../README.md)
