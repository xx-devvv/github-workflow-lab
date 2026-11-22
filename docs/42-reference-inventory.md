# 42. Record branch and tag pointers for a later comparison

Create a read-only baseline before an automated practice session.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git for-each-ref --format='%(refname) %(objectname)' refs/heads refs/tags
git rev-parse HEAD
```

Commit IDs make a precise comparison for the refs you actually inspected. A local snapshot does not prove remote refs are unchanged unless you separately inspect or fetch the remote state.

## Exercise

Save the output locally and compare it after a scratch exercise. Report the exact refs covered rather than claiming a broader audit.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-for-each-ref)

[Return to the lab index](../README.md)
