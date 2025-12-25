# Stashing

- Stashing
  - stashing uncommitted changes so that we can return to them later
  - We can add multiple stashes onto the stack of stashes .They will all be stashed in the order we add them ➡️stack
- Take all uncommitted changes and stash them reverting the changes in our working directory ➡️ `git stash`
- **Removes** the most recently stashed changes in our stash and re-apply them in our working directory ➡️ `git stash pop`
- Apply whatever is stashed without removing it from the stash (most recent) ➡️ `git stash apply`
- Viewing stashes ➡️ `git stash list`
- Applying a particular stash (say stash@{2}) ➡️ `git stash apply stash@{2}`
- Clearing the stash ➡️`git stash clear`
- Dropping a particular stash (say stash@{2}) ➡️`git stash drop stash@{2}`
- Stashing with a comment ➡️ `git stash push -m "WIP:refactor auth logic"`