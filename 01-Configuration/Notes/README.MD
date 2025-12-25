# Configuration

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