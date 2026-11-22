# 29. Export a reviewable working-tree patch

Save a textual diff for inspection without immediately applying it elsewhere.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git diff --output=practice-change.patch
git apply --stat practice-change.patch
git apply --check practice-change.patch
```

The default diff includes unstaged tracked changes. The patch is untracked until you add it and may contain sensitive content. --check asks whether application is possible; it does not apply the patch.

## Exercise

Inspect a patch in a scratch clone before sharing it. To check application against a clean destination, use a separate disposable clone.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-apply)

[Return to the lab index](../README.md)
