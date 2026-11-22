# 16. Diagnose line-ending differences

Separate meaningful content changes from carriage-return differences on Windows.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git config --show-origin --get core.autocrlf
git ls-files --eol -- README.md
git diff --ignore-space-at-eol -- README.md
```

An unset configuration key can return a nonzero exit code. ls-files reports index and working-tree line endings separately. Hiding whitespace differences is an inspection aid, not proof a patch is correct.

## Exercise

Read the existing .gitattributes first. Do not mass-normalize another project merely to make its diff quieter.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-ls-files)

[Return to the lab index](../README.md)
