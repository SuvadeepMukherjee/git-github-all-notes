# Code Along

## Git Configuration 

**Q1**:Code Along

1. Check the current git configuration (the effective value after local overrides global)
2. Change the git configuration globally 
3. Check the git configuration again (the effective value after local overrides global)
4. Now Change the git configuration locally 
5. Check the local configuration and   global  configuration 

**Solution**:

- **Current git configuration**(effective value after local overrides global):
  - `name : `git config user.name
  - `email : `git config user.email`
- **Change git configuration globally** 

  - name : `git config --global user.name "suvadeep"`
  - email : `git config --global user.email "suvadeepm0709@gmail.com"`
- **Check git configuration again**:
- name :`git config user.name`
  
- email : `git config user.email`
- **Change git configuration locally**

  - name : `git config --local user.name "suva"`
  - email : `git config  --local user.email "suva@gmail.com"`
  - Note ➡️ `git config --local user.name` only works inside a git repository
- **Check local configuration and global configuration**:

  - local configuration ➡️ `git config --local --list`
  - global configuration ➡️`git config --global --list`

Note ➡️ Local git configuration overrides global configuration 

## Basic Terminal Commands

**Q1**: Code Along

- List all files in the current directory
- List all files in a specific subdirectory
- Print current working directory
- Change folder to another directory
- Go up one directory
- Create a file called `index.js`
- Create a folder called `playground`
- Delete the file `index.js`
- Delete the folder `playground`
- List all files including hidden files

**Solution**:

- **List files in the current directory**
  - `ls`
- **List files in a specific subdirectory**
  - `ls <dir>`
- **Print current working directory**
  - `pwd`
- **Change folder to another directory**
  - `cd <directory>`
- **Go up one directory**
  - `cd ..`
- **Create a file called `index.js`**
  - `touch index.js`
- **Create a folder called `playground`**
  - `mkdir playground`
- **Delete the file `index.js`**
  - `rm index.js`
- **Delete the folder `playground`**
  - `rmdir playground`
  - (or `rm -rf playground` if the folder is not empty)
- **List all files including hidden files**
  - `ls -a`

##  Adding and Committing

### Adding and Committing

**Q1**: Code Along

- Make a folder called `temp`
- Move into the `temp` folder
- Initialise a Git repository
- Create 3 files `index.js`, `app.js`, `server.js`
- Add `index.js` to the staging area
- Check Git status
- Add `app.js` and `server.js` to the staging area with one command
- Check Git status again
- Commit all staged files with an inline commit message
- Check the logs both inline and detailed

**Solution**:

- Make a folder called `temp`
  - `mkdir temp`
- Move into the folder
  - `cd temp`
- Initialise Git repository
  - `git init`
- Create files
  - `touch index.js app.js server.js`
- Add `index.js` to staging area
  - `git add index.js`
- Check Git status
  - `git status`
- Add `app.js` and `server.js` to staging area
  - `git add app.js server.js`
- Check Git status again
  - `git status`
- Commit staged files with inline message
  - `git commit -m "add index.js, app.js and server.js"`
- Check git logs
  - one line : `git log --oneline`
  - detailed: `git log`

**Q**: Simulate entering and exiting Vim 

- Make a temporary folder `temp`
- cd into temp 
- make a file `hello.txt`
- open `hello.txt` with `vim hello.txt`
- Inside the editor write a message `Hello Vim`
- exit vim

**Solution**:

- make a temporary folder `temp` ➡️ `mkdir temp`
- cd into temp ➡️ `cd temp`
- make a file `hello.txt` ➡️ `touch hello.txt`
- `vim hello.txt`
- Vim Commands 
  - i ➡️ enter insert mode
  - Write `Hello Vim`
  - To exit vim ➡️ `Esc` the `:wq⏎ `
  - Tricks : ✅ **I Easily Eat Worms Quickly** ➡️`i`➡️Enter Commit Message ➡️ `ESC` ➡️ `:wq` ⏎

**Q**: Simulating Commit messages in default editor

- Create a temp folder called `temp`
- Change folder to `temp`
- Create  a file called `index.js`
- Open folder with Vs Code
- Edit `index.js` 
- Commit without inline message make the commit message `initial`
- Amend the commit message to be `initial commit`
- Check logs 

**Solution**:

- Creating a temp folder called `temp` ➡️ `mkdir temp`
- Change folder to `temp` ➡️ `cd temp`
- Create a file called `index.js` ➡️ `touch index.js`
- Open folder with Vs Code ➡️ `code .`
- Commit without inline message make the commit message `initial` ➡️ `git init`,`git add .`,`git commit` , Write in default editor `initial`
- Amend the commit message to be `initial commit` 
  - `git commit --amend`
    - This will open up default editor
    - Change `initial` to `initial commit`
    - Close the default editor  
- Check git logs ➡️`git log --oneline`
