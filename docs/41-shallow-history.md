# 41. Detect incomplete local history

Check whether a clone intentionally contains only part of the commit graph.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git rev-parse --is-shallow-repository
git log --oneline -5
```

A shallow clone can limit ancestry-based operations and history searches. The available log alone does not prove the upstream repository began at its oldest visible commit. Fetching more history changes local storage and uses network access.

## Exercise

Compare a separately created shallow scratch clone with a normal one. Request more history only when the investigation actually needs it.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-rev-parse)

[Return to the lab index](../README.md)
