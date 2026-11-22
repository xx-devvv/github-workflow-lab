# 25. Restore one tracked scratch file

Discard a deliberate practice edit without touching unrelated files.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git diff -- README.md
# This discards unstaged changes to this one file.
git restore -- README.md
git status --short
```

Restore can destroy uncommitted work. Its default working-tree source is the index, so staged content matters. Inspect the diff and preserve anything valuable before running it.

## Exercise

Make a disposable edit in a scratch clone, inspect it, and restore only that file. Never use this exercise on work you need to retain.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-restore)

[Return to the lab index](../README.md)
