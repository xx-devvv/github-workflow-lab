# 03. Stage only the intended files

Choose exactly what belongs in the next commit instead of including unrelated files.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git status --short
git add -- README.md
git diff --cached --stat
git diff --cached
```

The cached diff is what the next commit will contain. A file can have both staged and unstaged changes. Inspect both columns of git status, and avoid adding credentials or local configuration.

## Exercise

To unstage a file while preserving its working copy, run git restore --staged -- README.md. Use an existing tracked README in your scratch repository.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
