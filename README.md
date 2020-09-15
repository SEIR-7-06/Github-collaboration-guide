# Github Collaboration Workflow

## Set Up
- One team member will create the project repo.
- The repo owner will then add **Collaborators** to the repo.
- Owner will create the project **Boilerplate**.
    - Add, Commit, and push to **master** branch

- Owner create a new branch called **submaster**.
    - `git checkout -b submaster`
    - `git push origin submaster` to push **submaster** up to Github.

- Collaborators can now clone the project repo.
- Collaborators checkout to **submaster** branch.
    - `git checkout submaster`

- All Team members create their own working branch.
    - `git checkout -b <branch name>`

## Workflow
- Verify you are in our own branch.
    - `git branch`

- Make edits.
- Git add, Commit.
- Checkout **submaster** and verify branch is up to date.
    - `git checkout submaster`
    - `git pull origin submaster`
- **IF THERE ARE UPDATES** to **submaster** merge updates to working branch.
    - `git checkout <branch name>` (i.e. Kenny)
    - `git merge submaster`

- **IF THERE ARE NO UPDATES** to **submaster**, checkout your working branch and push to origin.
    - `git checkout <branch name>`
    - `git push origin <branch name>`

- Go to public repo on github and create a new pull request from **Your Branch** to **submaster**.
- Ask a team member to validate your pull request on github.
- **If all team mates agree** and **there are no conflicts** accept the pull request.
- Make sure everyone knows there are new changes available to be pulled down.
- **EVERYONE** save edits to working branch and and update all local branches.
    - `git add -A && git commit -m "message"` in working branch.
    - `git checkout master`
    - `git pull origin master` (resolve conflicts if any)
    - `git checkout submaster`
    - `git pull origin submaster` (resolve conflicts if any)
    - `git checkout <branch name>`
    - `git merge submaster`
- Repeat from the start of workflow
