# 09. Resolve a conflict deliberately

Understand both versions of an overlapping edit before completing a merge.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git status
git diff --name-only --diff-filter=U
git diff
git add -- README.md
git merge --continue
```

Use the final two commands only after editing every conflict marker in README.md into the intended final text. Check that the resulting document is correct, then continue. git merge --abort abandons an in-progress merge when Git can restore its starting state.

## Exercise

In a scratch repository, change the same README line differently on two branches and merge them. Inspect both commit versions before choosing the final wording.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
