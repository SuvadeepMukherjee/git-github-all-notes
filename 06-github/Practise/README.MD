## Github Practise

**Q**: `pr-conflict-practise` (High Priority)

- Create a git repo `pr-conflict-practise`

- Add a file `README.MD`

- Connect to Github  

- Add `suvadeep-ship-it` as a collaborator and open the github repo from `Suvadeep-ship-it` account

- From `suvadeep-ship-it`  account create a new branch `feature/add-line-from-b`

- Edit the README.MD to the following

  ```bash
   # Feature Branch Practice
  
    This line is added by Account B.
  
  ```

- Commit to branch:`feature/add-line-from-b`

- Open a  Pull Request from Account-B (suvadeep-ship-it)

- Create conflict on main (Account A , local), modify the same file locally 

  ```bash
  # Feature Branch Practice
  
  This line is added by Account A.
  ```

- Commit and push from main account 

- Confirm by opening the `pull-request` from main account github page and see that there are conflicts

- Resolve PR Conflict locally (Account A)

- Confirm the merge is completed 

**Solution**:

- Create a git repo `pr-conflict-practise` ➡️ `mkdir pr-conflict-practise` , `cd pr-conflict-practise` , `code .` , `git init`

- Add a file `README.MD` ➡️ Follow the instructions

- Connect to Github ➡️ Follow the instructions

- From `suvadeep-ship-it`  account create a new branch `feature/add-line-from-b` ➡️ Follow the instructions

- Edit the README.MD to the following ➡️ Follow the instructions

- Commit to branch:`feature/add-line-from-b` ➡️ Follow the instructions

- Open a  Pull Request from Account-B (suvadeep-ship-it) ➡️ Follow the instructions

- Create conflict on main (Account A , local), modify the same file locally  ➡️ Follow the instructions

- Commit and push from main account ➡️ Follow the instructions

- Confirm by opening the `pull-request` from main account github page and see that there are conflicts ➡️Follow the instructions

- Resolve PR conflict locally

  - Switch to the branch in question. Merge in main and resolve the conflicts

    ```
    git fetch origin 
    git switch feature/add-line-from-b
    git merge main 
    # fix conflicts!
    ```

  - Switch to main. Merge in the feature branch (now with no conflicts). Push changes up to Github

  - ```
    git switch main 
    git merge feature/add-line-from-b
    git push origin main
    ```

- Confirm the merge is completed  ➡️ Follow the instructions

**Q**: `raise-a-pull-request` demo (Low Priority)

- From the account `suvadeep-ship-it` create a repo `how-to-raise-a-PR-practise`
- edit the `README.MD` file create anything
- Add this account `SuvadeepMukherjee` (main account) as a collaborator from `suvadeep-ship-it`
- Accept the invitation from the main account(`SuvadeepMukherjee`) , clone it locally
- Add a new file locally name it `index.js` add whatever you want (locally)
- Create a new branch , add it , commit it , push the new branch, create a pull request
- Check from `suvadeep-ship-it` and you will see there is a new `PR`  

**Solution**:

- From the account `suvadeep-ship-it` create a repo `how-to-raise-a-PR-practise` ➡️ Follow the instructions
- edit the `README.MD` file create anything ➡️ Follow the instructions
- Add this account `SuvadeepMukherjee` (main account) as a collaborator from `suvadeep-ship-it` ➡️ Follow the instructions
- Accept the invitation from the main account(`SuvadeepMukherjee`) , clone it locally ➡️ Follow the instructions
- Add a new file locally name it `index.js` add whatever you want (locally) ➡️ Follow the instructions
- Create a new branch , add it , commit it , push the new branch, create a pull request ➡️ Follow the instructions
- Check from `suvadeep-ship-it` and you will see there is a new `PR` ➡️ Follow the instructions

**Q**: `oss-demo`

- Log in to `suvadeep-ship-it` on Github 

  - create a new repository :`oss-demo`

  - Edit the `README.md` to 

    ```bash
    OSS Demo Project
    
    This is a demo open source project.
    Contributions are welcome.
    ```

  - Commit directly to `main`

- Fork the repo

  - Log in to **`SuvadeepMukherjee`** on GitHub.
    - Go to: `https://github.com/suvadeep-ship-it/oss-demo`
    - Click Fork

- Clone your fork locally

- Open your clone with VSCode

- Add the upstream remote(original project)

- Verify the remotes

- Create and switch to a feature branch  `docs/add-contribution-guide`

- Make a meaningful change locally

  - Create a new file , `CONTRIBUTING.MD`

  - Add content:

    ```bash
    # Contributing Guide
    
    - Fork the repository
    - Create a feature branch
    - Commit clean changes
    - Open a pull request
    ```

  - Stage and commit 

    ```bash
    git add CONTRIBUTING.md
    git commit -m "Add contributing guide for new contributors"
    ```

- Push feature branch to your fork (origin)
- Create a Pull Request from `SuvadeepMukherjee`
- Review and merge as  maintainer(from `suvadeep-ship-it`)

**Solution**: 

- Log in to `suvadeep-ship-it` on Github  ➡️ Follow the instructions
- Fork the repo ➡️ Follow the instructions
- Clone your fork locally ➡️ Follow the instructions
- Open your clone with VSCode ➡️ Follow the instructions
- Add the upstream remote(original project) ➡️ `git remote add upstream https://github.com/suvadeep-ship-it/oss-demo.git`
- Create and switch to a feature branch  `docs/add-contribution-guide` ➡️ `git checkout -b docs/add-contribution-guide`
- Make a meaningful change locally ➡️ Follow the instructions
- Push feature branch to your fork (origin) ➡️`git push origin docs/add-contribution-guide`
- Create a Pull Request from `SuvadeepMukherjee` ➡️ Follow the instructions
- Review and merge as  maintainer(from `suvadeep-ship-it`) ➡️ Follow the instructions