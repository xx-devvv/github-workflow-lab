# 11. Copy a selected change to another branch

Apply one useful commit without merging every commit from its original branch.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git log --oneline practice/topic
git switch main
# Replace COMMIT_SHA with the one practice commit to copy.
git cherry-pick COMMIT_SHA
git show --stat HEAD
```

Cherry-picking normally creates a new commit with a different identity, even when the file change matches. It may conflict or become empty if the destination already contains the change. Do not use it merely to duplicate contribution credit.

## Exercise

Use a fresh topic commit not already on main. If an exercise becomes confusing, git cherry-pick --abort exits an in-progress operation before it is completed.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
