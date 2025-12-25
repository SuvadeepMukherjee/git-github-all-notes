# 02-Committing

- Initializing a git repo
  - `git init`
- Adding a file (say index.js) to staging area
  - `git add index.js`
- Commit all files to the staging area
  - `git add .`
- Commit all staged files with an inline commit message
  - `git commit -m "message"`
- Checking git logs
  - `git log`
  - `git log --oneline`
  - Note ➡️ If there are lots of git logs the command to exit pager : `q`
- Committing without any inline commit message
  - `git commit`
  - Opens `$EDITOR`; commit **fails** if message is empty
- Ammending the last commit message
  - `git commit --amend`

Note ➡️

- **Working Directory** is where files are edited.  **Staging Area** is where selected changes are prepared for commit using `git add`**Repository** stores committed snapshots using `git commit`

  ![git-workflow](https://github.com/SuvadeepMukherjee/git-github-all-notes/raw/main/assets/git-workflow.png)