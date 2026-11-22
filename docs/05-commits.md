# 05. Create a focused, attributable commit

Save a reviewable checkpoint with an accurate identity and message.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git config --local user.name
git config --local user.email
git diff --cached
git commit -m 'Document the practice workflow'
git show --stat --oneline HEAD
```

The commit contains the staged snapshot, not every changed file. Use a verified address or your GitHub-provided noreply address when you want contribution attribution. Credit collaborators only for work they actually contributed.

## Exercise

Read the final commit summary and confirm its file list matches the intended scope. Git configuration changes belong to this scratch repository, not unrelated projects.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
