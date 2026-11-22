# 39. Recognize submodule state

See which external repository revisions a parent project records.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git submodule status
git ls-files --stage
```

A submodule entry records another repository's commit ID rather than embedding its full working files. An empty submodule-status output is normal when none exist. Initializing submodules can contact external remotes.

## Exercise

Identify a mode 160000 entry if the scratch repository has a submodule. Do not initialize unfamiliar external code just to inspect the parent metadata.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-submodule)

[Return to the lab index](../README.md)
