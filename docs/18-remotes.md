# 18. Inspect fetch and push destinations

Check where a command will read from or write to before using a remote.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git remote -v
git remote get-url origin
git remote get-url --push origin
```

Fetch and push URLs can differ. A remote name such as origin is a local label, not evidence that a repository belongs to you. Treat URLs containing credentials as secrets.

## Exercise

Compare the displayed destination with the intended practice repository. Do not change remotes in an unrelated checkout.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-remote)

[Return to the lab index](../README.md)
