# Undoing Changes

**Q1**: View the contents of an old commit

**Solution**:

- `git checkout commit-hash`

Note ➡️ This will put us in detached HEAD

**Q2**: What is detached HEAD ? 

**Solution**:

- HEAD is a pointer to the current branch reference (branch reference is a pointer to the last commit made on a particular branch)
- When we do `git checkout commit-hash` HEAD points at that commit rather than at the branch pointer

**Q3**: How to reattach detached HEAD ? 

**Solution**:

- `git switch -` ➡️ This will switch back to wherever we were before

**Q4**: Restore the contents of a file to the state they were at the last commit ? 

**Solution**:

`git restore file`

(resrore) t  ➡️  **t**he ultimate (Control + Z)

(reset) e ➡️ **e**vent horizon (go back in time)

(revert) v ➡️ **v**ery good(as it is used in practise)  

**Q5**:

- Reset the repo back to a specific commit (only the commits are gone , changes are there)
- Reset the repo back to a specific commit(both the commits and changes are gone)➡️ `git reset --hard commit-hash`

**Solution**:

- Reset the repo back to a specific commit (only the commits are gone , changes are there) ➡️`git reset commit-hash`

- Reset the repo back to a specific commit(both the commits and changes are gone)➡️ `git reset --hard commit-hash`

(restore) t  ➡️  **t**he ultimate (Control + Z)

(reset) e ➡️ **e**vent horizon (go back in time)

(revert) v ➡️ **v**ery good(as it is used in practise)  

**Q6**: `git reset` vs `git revert`

**Solution**:

|                         | git reset                                                    | git revert                                                   |
| ----------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| What it does            | reset moves the branch pointer backwards eliminating commits | revert creates a brand new commit which reverses the changes from a commit(moves forward) |
| Where will it take us ? | the state of our repo at that commit-hash                    | the state of the repo after applying the inverse of that commit on top of the current branch |

(restore) t  ➡️  **t**he ultimate (Control + Z)

(reset) e ➡️ **e**vent horizon (go back in time)

(revert) v ➡️ **v**ery good(as it is used in practise)  

**Q7**: Explain the steps in git revert ? 

**Solution**:

- It will go to the state of the repo after applying the inverse of that commit on top of the current branch
- Fix Conflicts 
- Add and commit

