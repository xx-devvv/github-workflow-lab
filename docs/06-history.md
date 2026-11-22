# 06. Read history and inspect an individual change

Find when and why a change was introduced without modifying history.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git log --oneline --decorate --graph -12
git log --oneline -- README.md
git show HEAD -- README.md
git blame -- README.md
```

A path-limited log narrows the search to one file. Blame identifies the last commit touching a line; it is a starting point for investigation, not a measure of responsibility or quality.

## Exercise

Choose a line in README.md, find its commit with blame, and inspect the complete commit message and diff with git show.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
