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
git commit -am "add and commit"

git commit -a --amend "my comment"
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
git log

// options
--oneline // in one line style
--patch / -p
--decorate
--graph
-[2] // show last 2 commit

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

Display all branches (local and remote)

```
git branch -a

```

### Fetching and Pulling

Pull/fetch from local repository (from master branch)

```
git pull . master

git fetch . master
```
### Diffing Files

Compare a branch to another

```
git diff [branch-a] [branch-b] // difference viewed from both side

git diff [a]..[b]  // difference viewed from b (what changed in a, not in b)

--name-only // only the name of the files changed
--stat // brief description and short summary

```
### Merging branches

```
git branch

-d // delete
-D // force Delete

```
Fast-forward

### Tags

Tags like branches, you can check it out. It will restore the situation at that moment to the working directory.

Types of tags:
- Light-weight/simple
- Annotated

Add Tags

```
git tag [tag-name] // create tag from current HEAD.

git tag [tag-name] [hash-of-commit] // add tag to a commit earlier

-a // annotated

```

Switch to tag:
The working directory will be restore to the version of the tag. But the files are not lost (they are still kept in git repository)

```
git checkout [tag-name]

```

Remove tag
```
git tag -d [tag-name]
```

Show tag
```
git show [tag-name]
```

## GitHub and Remotes

Push changes to remote branches

```
git push [repository-name(origin)] [branch-name]

-u //upstream: set a tracking reference to the specified upstream branch

```

## Intermediate Usage

### Stashing changes
Stash:
- a stack that can take any number of stashes
- stored in reverse chronological order

When to stash
- has some changes on one branch and these changes are staged
- need to switch to another branch
- do not want to make commit to current branch, and do not want to lost the changes

Save stash
```
git stash

git stash save "description of the stash"

```
Show stash:

```
git stash show stash@{0}

```

Compare stashes

```
git diff stash@{0}...stash@{1}
```

Remove stash

```
git stash drop @stash@{0}

git stash clear // remove all the stashes

```

### Cleaning Up Merge Conflicts

### Rebasing

When to use rebase
- squash multiply commits to one commit (on same branch), to make the git history concise
- avoid pointless merging when merge changes from another branch

```
git rebase [hash-of-commit]

-i // interactive

```
