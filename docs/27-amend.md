# 27. Correct the latest unpublished commit

Combine a small follow-up with a commit that has not been shared.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git diff --cached
git commit --amend --no-edit
git show --stat HEAD
```

Amend creates a replacement commit even when its message stays the same. It incorporates staged changes and changes the commit hash. Do not use it as a routine way to rewrite published work.

## Exercise

On a scratch branch, stage a typo fix for the latest local commit. Compare its old and new hashes after amending.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-commit)

[Return to the lab index](../README.md)
