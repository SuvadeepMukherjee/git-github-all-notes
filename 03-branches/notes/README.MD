# Branches

- View your existing branches ➡️`git branch`

- To exit out of the window showing all the branches(if it shows in full screen)  ➡️`q`

- Create a new branch (does not switch to that branch) ➡️ `git branch branchName`

- Switch to an existing branch ➡️ `git switch branchName`

- Create and switch to a new branch ➡️ `git checkout branch -b branchName`

- Renaming a branch ➡️ `git branch -M newName`(We must be on the branch we want to rename)

- Deleting a branch ➡️ 

  ```
  git branch -d branchToDelete
  ```

  - We cannnot delete a branch that's not fully merged
  - We cannot delete the branch if we are on it

## Merging Branches



- To merge 2 branches follow the few steps
  - Switch to the branch you want to merge the changes into (the receiving branch) with `git switch`
  - Use `git merge` to merge changes from the specific branch into the current branch
- Fast Forward Merge
  - A fast-forward merge can occur when there is a linear path from the current branch tip to the target branch
  - Instead of actually merging the branches , all Git has to do to   integrate the histories is move (i.e "fast forward") the current branch  tip up to the target branch tip![![fast-forward](https://github.com/SuvadeepMukherjee/git-github-all-notes/raw/main/assets/fast-forward.gif)](https://github.com/SuvadeepMukherjee/git-github-all-notes/blob/main/assets/fast-forward.gif)      
- No conflict merges
  - git performs a merge commit
  - We end up with a new commit on the master branch
  - Git will prompt us for a commit message on our default code editor
- Merges with conflicts
  - When you encounter a merge conflict ,Git warns you in the console that it could not automatically merge
  - It also changes the contents of our files to indicate the conflicts that it wants you to resolve
  - Resolving Conflicts
    - Open up the file(s) with merge conflicts
    - Edit the file(s) to remove the conflicts.Decide which branch's   content you want to keep in each conflict or keep the content from both
    - Remove the conflict "markers" in the document
    - Add your changes and then make a commit!