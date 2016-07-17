# Git Tips and Tricks

```
git count-objects
git cat-file -p [my-tag-name/tag-hash] // provide git object information (i.c. tag)
git ls-files  // show info about files in the index 
```
To put a file to *staging area*:
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

git checkout -- [my-file]

```

Unstage files

```
git reset HEAD // remove all files from staging area, and point to latest commit

git reset HEAD -- [file/path]

git reset --hard // revert all changes

```

Go to a commit
```
git checkout [hash-of-the-commit]
```

Display content of compressed file

```
git cat-file -p [hash-of-an-object]
```

## Questions
