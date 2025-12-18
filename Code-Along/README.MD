# Code Along

## Git Configuration and Basic Terminal Commands

**Q2**:Code Along

1. Check the current git configuration 
2. Change the git configuration globally 
3. Check the git configuration again
4. Now Change the git configuration locally 
5. Check again whether the git configuration is correct locally and globally (You can check the local configuration at that folder level and global git configuration by going up one level)? 

**Solution**:

- **Current git configuration**:

  - `name : `git config user.name`

  - email : `git config user.email`

- **Change git configuration globally** 

  - name : `git config --global user.name "suvadeep"`
  - email : `git config --global user.email "suvadeepm0709@gmail.com"`

- **Change git configuration locally**
  - name : `git config --local user.name "suva"`
  - email : `git config  --local user.email "suva@gmail.com"`

Note ➡️ git configuration is overriden by `local` over `global` 

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



