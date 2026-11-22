# 01. Inspect a repository before changing it

Establish the current branch, working-tree state, and remotes before starting work.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git status --short --branch
git branch --show-current
git remote -v
git log -5 --oneline
```

An empty short-status listing means the working tree is clean. A remote URL identifies a destination; it does not prove permission to push. Stop and understand unexpected changes before editing.

## Exercise

Record the branch and latest commit in your notes. None of these commands changes tracked files.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
