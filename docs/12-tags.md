# 12. Label a known revision with an annotated tag

Give a tested or reviewed snapshot a memorable local name.

Run these commands only in a disposable practice clone. These are independent exercises; prepare the named branches or edits first.

```powershell
git tag -a practice-v0.1 -m 'First reviewed practice snapshot'
git show practice-v0.1
git tag --list
```

A tag names a commit; an annotated tag also carries a message and identity. A local tag is not automatically a GitHub release and is not pushed by an ordinary branch push. Reusing a published tag can confuse consumers.

## Exercise

Inspect the tag before publishing it. If publication is intended, push only that explicit tag instead of every local tag.

## Reference

[Git command documentation](https://git-scm.com/docs)

[Return to the lab index](../README.md)
