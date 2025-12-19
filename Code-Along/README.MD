# Code Along

## Git Configuration and Basic Terminal Commands

**Q1**:Code Along

1. Check the current git configuration (the effective value after local overrides global)
2. Change the git configuration globally 
3. Check the git configuration again
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

- **Check local configuration and global configuration**:

  - local configuration ➡️ `git config --local --list`
  - global configuration ➡️`git config --global --list`

Note ➡️ Local git configuration overrides global configuration 

**Q2**: Code along 

- list all files in your  directory and all files in a sub directory
- print current working directory
- change folder to another directory 
- go up one directory 
- create a file called `index.js`
- create a folder called `playground`
- delete the file `index.js`
- delete the folder `playground`
- List all files including hidden files

**Solution**:

- list all files in your directory and all files in a sub directory 
  - `ls` , `ls <dir>`
- print current working directory 
  - `pwd`
- Change folder to another directory
  - `cd <directory>`
- Go up one directory 
  - `cd ..`
- create a file called `index.js`
  - `touch index.js`
- create a folder called playground
  - `mkdir playground`
- delete the file index.js
  - `rm index.js`
- delete the folder playground
  - `rm -rf playground`
- list all files including hidden files
  - `ls -a`

## Adding and Committing

**Q1**: Code Along

- make a folder called `temp`
- git initialise that folder 
- make 3 files `index.js` , `app.js`, `server.js`
- add `index.js` to staging area 
- check git status
- add `app.js` and `server.js` to the staging area with one command
- again check git status 
- now commit `index.js`, `app.js` and `server.js` from staging area to repository with a inline commit message 

**Solution**:

-  make a folder called `temp` ➡️ `mkdir temp`
- git initialise that folder ➡️ `git init`
- make 3 files `index.js`, `app.js` , `server.js` ➡️ `touch index.js app.js server.js`
- add index.js to staging area ➡️ `git add index.js`
- check git status ➡️ `git status`
- add `app.js` and `server.js` to the staging area with one command ➡️`git add .`
- Check git status ➡️ `git status`
- commit `index.js` , `app.js` and `server.js` from staging area to repository with an inline commit message ➡️ `git commit -m "add index.js,app.js and server.js to repository"`

