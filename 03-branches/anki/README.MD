# Anki Notes - Branches

**Q**: Command to view your existing branches 

**Solution**: `git branch`

**Q**: If `git branch` shows all the branches in full screen what's the command to exit ? 

**Solution**: `q`

**Q**: Create a new branch and switch to that branch using 2 different commands 

**Solution**:

- `git checkout branch -b branchName`
- `git switch -c branchName`

**Q**: git command to rename a branch assuming we are on the branch we want to rename 

**Solution**: `git branch -M newBranchName`

**Q**: git command to delete a branch assuming we are not on the branch we want to delete and the branch is fully merged 

**Solution**:

`git branch -d branchToDelete`

**Q**: Command to switch branches 

**Solution**: `git switch branchName`

**Q**: What is the process to merge 2 branches ? 

**Solution**:

- Switch to the branch you want to merge the changes into using `git switch`
- Use `git merge` to merge changes from that specific branch into the current branch

**Q**: What happens during a  Fast Forward merge in Git ? 

**Solution**:

Git moves the current branch pointer forward to the target branch tip without creating a merge commit

**Q**: What happens in a no-conflict merge in Git ? 

**Solution**:

Git creates a new merge commit and prompts for a commit message

Make it into close deletions card: 

In a no-conflict Git merge, Git creates a {{c1::new merge commit}} and prompts for a {{c2::commit message}}.

**Q**: What should you do when Git reports a merge conflict?

**Solution**:

Manually edit the conflicted files to resolve conflicts, remove conflict markers, then add and commit the changes

Make it into close deletions card: 

When Git reports a merge conflict, you must {{c1::manually edit the conflicted files}}, {{c2::remove conflict markers}}, then {{c3::add and commit the changes}}.