# 10. Undo a published change with a new commit

Reverse a specific change while preserving a shared history trail.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git log --oneline -5
# Replace COMMIT_SHA with the scratch commit to reverse.
git revert --no-edit COMMIT_SHA
git show --stat HEAD
```

A revert adds a new inverse change. It does not remove the original commit from history and can conflict with later work. Reverting a merge requires additional parent selection and is outside this small exercise.

## Exercise

Revert a simple practice-only commit, then compare the old and new history. Review the resulting files as carefully as a normal change.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
