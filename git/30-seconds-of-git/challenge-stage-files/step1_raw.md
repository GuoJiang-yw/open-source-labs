---
title: Add files to the staging area
---

Adds files to the staging area.

- Use `git add <pathspec>` to add files to the staging area.
- `<pathspec>` can be a filename or a fileglob.

```shell
git add <pathspec>
```

```shell
git add "labex.txt"
# Add the file `labex.txt` to the staging area

git add src/*.json
# Add all files with a `.json` extension in the `src` directory

git add .
# Adds all changes to the staging area
```
