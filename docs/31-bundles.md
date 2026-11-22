# 31. Create and verify a portable Git bundle

Package reachable repository objects and references for an offline handoff.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git bundle create ../workflow-lab.bundle --all
git bundle verify ../workflow-lab.bundle
git bundle list-heads ../workflow-lab.bundle
```

A bundle can contain private history and deleted secrets still reachable from included refs. It does not include uncommitted working files, Git LFS payloads, or submodule repositories automatically.

## Exercise

Use only a public scratch repository. Review the listed refs before handing the bundle to anyone.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-bundle)

[Return to the lab index](../README.md)
