# Github Collaboration Workflow

## Set Up
- One team member will create the project repo.

- The repo owner will then add **Collaborators** to the repo.

- Owner will create the project **Boilerplate**.

    - Add, Commit, and push to **main** branch

- Collaborators can now clone the project repo.

## Workflow for Adding a Feature

- Verify you are on the main branch
    - `git branch`

- Create a new working branch of off the main branch
    - `git checkout -b <branch name>`

- Make edits.

- Git add, Commit.

- Checkout **main** and verify the **main** branch is up to date.
    - `git checkout main`
    - `git pull origin main`

- **IF THERE ARE UPDATES** to **main** merge updates to your working branch.
    - `git checkout <branch name>` (i.e. your working branch)
    - `git merge main`
    - `git push origin <branch name>`

- **IF THERE ARE NO UPDATES** to **main**, checkout your working branch and push to origin.
    - `git checkout <branch name>`
    - `git push origin <branch name>`

- Go to public repo on github and create a new pull request from **Your Branch** to **main**.

- Ask a team member to verify the work in your pull request looks good.

- **If all team mates agree** and **there are no conflicts** merge the pull request.

- Make sure everyone knows there are new changes available to be pulled down.

- **EVERYONE** save edits to their working branch and and update all local branches.

    - `git add -A && git commit -m "message"` in working branch.

    - `git checkout main`

    - `git pull origin main` (resolve conflicts if any)

    - `git checkout <branch name>`

    - `git merge main`

- Repeat from the start of workflow
