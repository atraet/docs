# Git Tips and Tricks

To put a file to *stating area*:
```
git add [my-file]

```
## Important
- a new file added in branch-1, and it will be committed in branch-2, if it's switch to branche-2

- if a file is already added, but not staged, you can combine staging and commit in one command
```
git commit -am "my message"
```

To stage a file
```
git add . // add all changed file to staging area

git checkout -- my-file-name

```

Unstage files

```
git reset HEAD // remove all files from staging area

```

## Questions
