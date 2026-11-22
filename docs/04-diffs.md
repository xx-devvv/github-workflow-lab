# 04. Compare working, staged, and committed changes

Distinguish the three common comparisons before reviewing a change.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git diff
git diff --cached
git diff HEAD
git diff --check
```

git diff compares working files with the index; --cached compares the index with HEAD; diff HEAD compares tracked working files with HEAD. Untracked files do not appear until added. --check reports whitespace errors.

## Exercise

Stage one edit, make a second edit in the same file, and compare the first three outputs. Explain why they differ before committing.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
