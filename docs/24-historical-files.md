# 24. Read a file from an earlier revision

Inspect historical content without checking out or replacing a working file.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git show HEAD:README.md
git show 'HEAD~1:README.md'
git ls-tree --name-only HEAD
```

Revision:path addresses a file inside a commit. HEAD~1 requires a parent commit, and a path can be absent at that revision. These inspection commands do not restore or overwrite the current file.

## Exercise

Find a line added recently, inspect the earlier README, and explain why the current working copy remains unchanged.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-show)

[Return to the lab index](../README.md)
