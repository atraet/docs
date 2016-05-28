# Introduction to Git and GitHub

## Git Basics

### Initializing a Repository

```
git config --local user.name "Zhiping Liu"

git init

git init "my-project"

```
### The Staging Area

Staging area:
- intermediate step between untracked and tracked files;
- or: between un-added and added files that has changed.

### Making Commits

Combine add and commit in one single command:
```
git commit -am "add and commit" ???

git commit -a --amend "my comment" ???
```
### Ignoring files
Edit global git configuration
```
git config --global --edit
```
- how to ignore files and folders
- can ignore globally and locally

### Viewing the log
```
git log --oneline
git log -2 --online // show last 2 commit in oneline style
git log -p // patch
git log --decorate

```

## Branching and Tagging

### Create branch

Create a new branch

```
git branch [new-branch]

```

Switch to a branch

```
git checkout [my-branch]

```

Create a new branch and switch to it

```
git checkout -b [my-new-branch]

```

Delete a branch

```
git branch -d [my-branch]

```

Dislay all branches (local and remote)

```
git branch -a

```

### Fetching and Pulling

Pull from local repository (from master branch)

```
git pull . master
```

### Tags

Add Tags

```
git tag <tag-name> //

git tag -a <tag-name> <hash-of-commit> // add tag to a commit earlier
```

Get content of tag.
The working directory will be restore to the version of the tag. But the files are not lost (they are still kept in git repository)

```
git checkout <tag-name>
```

Remove tag
```
```

Show tag
```
show tag <tag-name>
```


To stage a file
```
git checkout -- my-file-name
```
