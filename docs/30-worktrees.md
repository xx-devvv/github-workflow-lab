# 30. Create a second working directory for a different branch

Work on another task without changing the files in the first checkout.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git worktree list
git worktree add ../workflow-lab-second -b practice/second main
git worktree list
```

Choose a new, unused sibling directory. Worktrees share a repository's object store and refs but have separate checked-out files and indexes. Git normally prevents checking out the same branch twice.

## Exercise

Keep the second worktree clean. When finished, inspect its status and use git worktree remove with its exact path rather than manually deleting a possibly dirty directory.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-worktree)

[Return to the lab index](../README.md)
