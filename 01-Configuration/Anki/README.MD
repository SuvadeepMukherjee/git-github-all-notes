# 01-Configuration

Anki : 01-configuration

**Q1**: How do you check the current git configuration (the effective value after local overrides global : name and email)

**Solution**:

- name : `git config user.name`
- Email: `git config user.email`

**Q2**: How do you change the git configuration globally ? 

**Solution**:

- name : `git config --global user.name "suvadeep"`
- Email: `git config --global user.email "suvadeepm0709@gmail.com"`

**Q3**: How do you change git configuration locally ? 

**Solution**:

- name : `git config --local user.name "suva"`
- Email : `git config --local user.email "suva@gmail.com"`

Note ➡️ Local Configuration can only be checked inside a git repo

**Q4**: How to check local configuration and global configuration ? 

**Solution**: 

- local configuration : `git config --local --list`
- global configuration: `git config --global --list`

