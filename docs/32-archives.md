# 32. Export a tracked snapshot without Git history

Produce an archive of files belonging to a chosen revision.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git archive --format=zip --output=../workflow-lab-snapshot.zip HEAD
git ls-tree -r --name-only HEAD
```

An archive omits the .git directory and untracked working files. Attributes such as export-ignore can affect its contents. Submodule contents and LFS payload handling need separate consideration.

## Exercise

Compare the archive's filenames with the tracked tree. Do not describe a source archive as a complete history backup.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-archive)

[Return to the lab index](../README.md)
