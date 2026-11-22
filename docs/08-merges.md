# 08. Understand a fast-forward merge

Integrate a topic branch when the destination has not advanced independently.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git switch main
git merge --ff-only practice/topic
git log --oneline --decorate -5
```

A fast-forward moves the branch pointer to an existing descendant commit. --ff-only refuses if histories have diverged, which is useful when a workflow expects a linear update. It does not invent a merge commit.

## Exercise

Perform this after creating a committed change on practice/topic. A refusal is information to inspect, not a reason to force an update.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
