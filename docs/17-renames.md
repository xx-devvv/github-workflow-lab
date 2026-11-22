# 17. Rename a tracked document deliberately

Move a file while keeping its content change easy to review.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
# Use disposable filenames that exist in your scratch clone.
git mv -- draft-note.md reviewed-note.md
git diff --cached --summary
git status --short
```

git mv stages the move. Git represents snapshots and detects renames from similarity; a rename is not a permanently stored file identity. Large simultaneous rewrites can make that detection less clear.

## Exercise

Create and commit draft-note.md in a scratch repository first. Rename it without editing the body, then inspect the staged summary.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-mv)

[Return to the lab index](../README.md)
