# 13. Recover a recent commit using the reflog

Find an earlier local position and preserve it without immediately rewriting a branch.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git reflog -10
# Replace COMMIT_SHA with the revision you inspected.
git show --stat COMMIT_SHA
git branch recovered-practice COMMIT_SHA
git log --oneline recovered-practice -5
```

The reflog records local reference movements and is not a permanent remote backup. Entries expire and missing objects may eventually be pruned. Creating a recovery branch preserves a reachable revision while leaving the current branch in place.

## Exercise

Inspect a recent reflog entry and create a recovery branch only when it names the version you actually want. Avoid destructive reset commands during this exercise.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
