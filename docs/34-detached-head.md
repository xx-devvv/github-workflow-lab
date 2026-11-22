# 34. Understand and preserve detached-HEAD work

Inspect a revision directly while knowing how to keep any new commits.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
# Replace COMMIT_SHA with a revision from the scratch history.
git switch --detach COMMIT_SHA
git status --short --branch
# If you create commits worth keeping, name a branch here.
git switch -c practice/inspection
```

Detached HEAD points directly at a commit rather than a branch name. New commits can become difficult to find when you leave without a reference. A branch name preserves a reachable tip.

## Exercise

Inspect an earlier commit in a clean scratch worktree. Decide whether to return to main or keep new work on a named branch.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-switch)

[Return to the lab index](../README.md)
