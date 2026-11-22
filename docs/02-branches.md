# 02. Create an isolated topic branch

Keep a focused change separate from the default branch.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git switch main
git switch -c practice/topic
git branch --show-current
```

The final command should print practice/topic. Creating a branch does not copy a directory: it creates another name pointing to a commit. Uncommitted changes may follow you between branches.

## Exercise

Make one small practice change on the topic branch. Return to main only after committing or deliberately saving that change.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
