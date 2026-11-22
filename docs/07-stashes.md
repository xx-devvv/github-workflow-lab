# 07. Temporarily save tracked work

Put a small unfinished change aside without pretending it is ready for a permanent commit.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git stash push -m 'practice work in progress'
git stash list
git stash show --patch 'stash@{0}'
git stash apply 'stash@{0}'
```

The default stash saves tracked changes, not untracked files. apply preserves the stash entry and may produce conflicts. In PowerShell, quote stash references containing braces. Review the restored files before deleting a stash.

## Exercise

Run this only after making a tracked scratch-file edit. To include untracked scratch files, use -u intentionally; never assume ignored files are included.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
