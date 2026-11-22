# 40. Inspect sparse working-tree configuration

Understand why tracked files may be absent from a deliberately partial checkout.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git sparse-checkout list
git config --get core.sparseCheckout
git ls-tree --name-only HEAD
```

The first command can fail when sparse checkout is disabled, and an unset configuration key can also return a nonzero status. Sparse checkout controls which tracked paths populate a working tree; it is different from shallow history.

## Exercise

Compare a normal scratch clone with a separately prepared sparse clone. Avoid enabling sparse checkout in an existing project as an unexplained fix for missing files.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-sparse-checkout)

[Return to the lab index](../README.md)
