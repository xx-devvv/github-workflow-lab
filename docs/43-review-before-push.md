# 43. Review scope before publishing a branch

Combine the status, file-list, whitespace, and destination checks into one practical pre-push review.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git status --short --branch
git diff --check main...HEAD
git diff --stat main...HEAD
git diff --name-only main...HEAD
git remote get-url --push origin
```

These checks cover the selected comparison and destination. They do not scan all history for secrets or prove behavioral correctness. Read the actual diff and run checks appropriate to code changes before publishing.

## Exercise

Apply the checklist to a scratch topic branch. Confirm every changed file belongs to the intended task and that the remote is the sandbox you meant to use.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-push)

[Return to the lab index](../README.md)
