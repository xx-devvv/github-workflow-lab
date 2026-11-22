# 36. List exactly what the repository tracks

Check scope without accidentally treating local generated files as committed source.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git ls-files
git ls-files -- '*.md'
git status --short --untracked-files=all
```

ls-files lists index entries, which can differ from both HEAD and the working tree during an edit. Quoting the wildcard lets Git interpret the pathspec rather than relying on the shell.

## Exercise

Create an untracked scratch file and compare these outputs. Explain why it is visible to status but absent from the tracked inventory.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-ls-files)

[Return to the lab index](../README.md)
