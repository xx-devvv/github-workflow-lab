# 22. Count commits on each side of a branch comparison

Measure ahead and behind using a specific pair of revisions.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git fetch origin
git rev-list --left-right --count HEAD...origin/main
git log --left-right --oneline HEAD...origin/main
```

The first count belongs only to HEAD; the second belongs only to origin/main. The symmetric difference includes commits reachable from either side but not both. Fetch first when current remote state matters.

## Exercise

Compare the counts with the left/right log. Avoid equating commit counts with the number or size of file changes.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-rev-list)

[Return to the lab index](../README.md)
