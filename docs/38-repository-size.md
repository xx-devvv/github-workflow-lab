# 38. Inspect repository object storage

Understand packed objects before blaming working-tree file sizes for clone cost.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git count-objects -vH
git rev-list --count HEAD
```

count-objects describes local object storage, while rev-list counts reachable commits from the selected tip. Neither command reports a hosted provider's billed storage or measures every external LFS object.

## Exercise

Record these values in a scratch clone. Do not run aggressive garbage collection or delete object files merely to improve the displayed numbers.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-count-objects)

[Return to the lab index](../README.md)
