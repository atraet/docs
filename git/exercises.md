# Exercises

### Resolving merge conflicts
- create a new branch 'working' from branch 'master'
- make some changes on 'working' and commit it
- switch to 'master'
- make some changes on 'master' and commit it
- merge into 'master' from 'working'
- you get merge conflicts
- edit the conflicts
- make commit of resolved conflicts

- delete 'working' branch
- DONE!

### Amending last commit
- create a new branch 'working' from branch 'master'
- make some changes on 'working' and commit it
  ```
  git commit --amend -am "this commit will replace the last one"
  ```

### Stashing uncommitted changes and store them back
  - on 'working' branch, make some changes
  - stash the changes
    ```
      git stash
    ```
  - switch to 'master' branch, make some changes
  - make commit on 'master' branch
  - switch to 'working' branch, unstash to get back the changes made before
    ```
    git stash apply stash@{0}
    ```
