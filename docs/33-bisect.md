# 33. Locate a regression with a binary search

Choose the first bad revision by repeatedly classifying checked-out commits.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git bisect start
# Replace these with known revisions in a scratch history.
git bisect bad BAD_SHA
git bisect good GOOD_SHA
# After testing each selected revision, mark it good or bad.
git bisect reset
```

Bisect changes the checked-out revision, often into detached HEAD. Begin with a clean scratch worktree. Classification must be reliable; skip revisions that cannot be tested instead of guessing.

## Exercise

Construct a small local history with a known document regression and manually classify each candidate. Finish with reset even if you abandon the search.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-bisect)

[Return to the lab index](../README.md)
