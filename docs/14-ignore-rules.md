# 14. Understand ignore rules and tracked files

Keep generated and private local files out of future commits.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git status --short --ignored
git check-ignore -v -- .env
git ls-files -- .env
```

.gitignore affects untracked files. It does not remove an already tracked file or erase a secret from history. A nonzero check-ignore exit code can simply mean no rule matched.

## Exercise

In a scratch clone, create an untracked .env with dummy text and verify the matching ignore rule. Never put a real credential in an exercise.

## Reference

[Official Git documentation](https://git-scm.com/docs/gitignore)

[Return to the lab index](../README.md)
