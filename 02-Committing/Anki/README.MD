# 02-Committing

Anki ➡️ 02-committing

**Q1**: git command to intialise a git repo ? 

**Solution**:

git command to initialise a git repo ➡️ `git init`

**Q2**: Adding a file (say index.js) to the staging area ?

**Solution**:

git command to add a file (say index.js) to the staging area ➡️ `git add index.js`

**Q3**: git command to add all files to the staging area ?

**Solution**:

git command to add all files to the staging area ➡️ `git add .`

**Q4**: Commit all staged files with an inline commit message 

**Solution**:

Commit all staged files with an inline commit message ➡️`git commit -m "message"`

**Q5**: git command to check git logs 

**Solution**:

- `git log`
- `git log --oneline`

Note ➡️ If there are a lot of git logs the command to exit pager : `q`

**Q6**: git command to commit without any inline commit message 

**Solution**:

- `git commit`
- Opens `$EDITOR`; commit **fails** if message is empty

**Q7**: git command to amend the last commit message 

**Solution**:

- `git commit --amend`

**Q8**: What is working directory , staging area and repository ? 

**Solution**:

![git-workflow](https://github.com/SuvadeepMukherjee/git-github-all-notes/raw/main/assets/git-workflow.png)

**Working Directory** is where files are edited.  **Staging Area** is where selected changes are prepared for commit using `git add`**Repository** stores committed snapshots using `git commit`