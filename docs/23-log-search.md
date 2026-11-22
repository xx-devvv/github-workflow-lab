# 23. Search history by message or changed text

Use different searches for commit descriptions and content changes.

Use a disposable practice clone. These are independent exercises, and their named paths, branches, and revisions need to exist before you use them.

```powershell
git log --oneline --grep='practice'
git log --oneline -S 'workflow' -- README.md
git log --oneline -G 'workflow.*lab' -- README.md
```

--grep searches commit messages. -S finds changes to the number of occurrences of a string; -G searches added or removed lines matching a regular expression. They answer different questions.

## Exercise

Choose a word from a document and compare the three search results. Inspect a matching commit before drawing a conclusion.

## Reference

[Official Git documentation](https://git-scm.com/docs/git-log)

[Return to the lab index](../README.md)
