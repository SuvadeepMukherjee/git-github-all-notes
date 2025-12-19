# Git & Github Cheat Sheet

## Git Configuration

- Check current git configuration (the effective value after local overrides global)
  - name : `git config user.name`
  - email : `git config user.email`
- Changing git configuration globally 
  - name : `git config --global user.name "suvadeep"`
  - email : `git config --global user.email "suvadeepm0709@gmail.com"`
- Changing git configuration locally 
  - name : `git config --local user.name "suva"`
  - email : `git config --local user.email "suva@gmail.com"`
  - Note ➡️ local configuration can only be checked inside a git repo 

- Check local configuration 
  - `git config --local --list`
- Check Global Configuration 
  - `git config --global --list`

## Basics of Adding and Committing

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

Note ➡️

- **Working Directory** is where files are edited.  **Staging Area** is where selected changes are prepared for commit using `git add`**Repository** stores committed snapshots using `git commit`

  <img src="../assets/git-workflow.png" alt="git-workflow" style="zoom:100%;" />

  

