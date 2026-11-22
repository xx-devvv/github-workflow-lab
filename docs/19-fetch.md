# 19. Fetch remote state without merging it

Update remote-tracking references while leaving the checked-out branch in place.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git status --short --branch
git fetch origin
git log --oneline --decorate -5 origin/main
git status --short --branch
```

Fetch downloads reachable objects and updates configured remote-tracking refs. It does not normally integrate those commits into the current local branch or rewrite working files.

## Exercise

Record the local HEAD before and after a fetch. Distinguish your branch tip from origin/main when they differ.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-fetch)

[Return to the lab index](../README.md)
