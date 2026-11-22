# 15. Inspect per-file Git attributes

See which line-ending or diff rules apply to a path.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git check-attr --all -- README.md
git check-attr text eol -- README.md
```

Attributes come from .gitattributes and other configured sources. Inspect effective values before changing rules. Adding attributes does not by itself rewrite every historical commit.

## Exercise

Compare README.md with a new scratch binary filename. Explain the difference between an unspecified attribute and an explicit value.

## Reference

[Official Git documentation](https://git-scm.com/docs/gitattributes)

[Return to the lab index](../README.md)
