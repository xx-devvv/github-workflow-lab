# 35. Follow a document through a rename

Investigate earlier versions when a file's current path is new.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
# Replace the path with a renamed tracked scratch document.
git log --follow --oneline -- reviewed-note.md
git log --name-status --oneline -5
```

--follow is for one file and uses rename detection. It is a useful heuristic, not a complete identity history for arbitrary rewrites, copies, and complex merges.

## Exercise

Rename a committed scratch file and compare a plain path log with --follow. Inspect a candidate commit to confirm the connection.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-log)

[Return to the lab index](../README.md)
