# 37. Inspect the objects behind a commit

Distinguish commit metadata, directory trees, and file blobs.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git cat-file -t HEAD
git cat-file -p HEAD
git rev-parse 'HEAD^{tree}'
git ls-tree HEAD
```

A commit refers to a tree and parent commits. A tree maps names to objects; a blob stores file content. These plumbing commands expose the model without modifying any references.

## Exercise

Find README.md's blob ID in the tree, then inspect that object with cat-file. Keep object content private when practicing on nonpublic data.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-cat-file)

[Return to the lab index](../README.md)
