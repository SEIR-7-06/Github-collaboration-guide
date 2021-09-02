# Github Collaboration Workflow

For this activity we will work in pairs.

## Set Up
1. Have Team Member A create a brand new repo in Github.
    - Make it public
    - do not add a readme or any files on initialization

1. Team Member A can then add **Collaborators** to the repo.
    - settings tab > Manage access > Invite a collaborator
    - search for your partner by their Github username
    - add your partern
    - Team Member B can then check their email and accept the invitation

1. Have Team Member A create the project boilerplate.
    - Team Member A clones down the repo to their local machine.
    - Team Member A creates an HTML file and adds some basic code.
    - Add and commit your work.
    - `git push origin main`

1. Have Team Member B clone down the project.

## Workflow for Adding a Feature

Pick one team member to go through the following steps to add a feature.

- verify you are on the main branch
    - `git branch`

- create a new working branch of off the main branch
    - `git checkout -b <branch name>` (replace `<branch name>` with what you'd like to name your branch)

- make edits.

- Git add, Commit.

- checkout **main** and verify the **main** branch is up to date.
    - `git checkout main`
    - `git pull origin main`

- **IF THERE ARE UPDATES** to **main** merge updates to your working branch.
    - `git checkout <branch name>` (i.e. your working branch)
    - `git merge main`
    - `git push origin <branch name>`

- **IF THERE ARE NO UPDATES** to **main**, checkout your working branch and push to origin.
    - `git checkout <branch name>`
    - `git push origin <branch name>`

- go to public repo on github and create a new pull request from **Your Branch** to **main**.

- ask a team member to verify the work in your pull request looks good.

- **If all team mates agree** and **there are no conflicts**, Team Member B merge the pull request.

- Make sure everyone knows there are new changes available to be pulled down.

- **EVERYONE** (including Team Member B) save edits to their working branch and and update all local branches.

    - `git add -A && git commit -m "message"` in working branch.

    - `git checkout main`

    - `git pull origin main` (resolve conflicts if any)

    - `git checkout <branch name>` (your working branch)

    - `git merge main`

Repeat [Workflow for Adding a Feature](#workflow-for-adding-a-feature) with the other team member. Continue alternating [Workflow for Adding a Feature](#workflow-for-adding-a-feature) with one team member adding a feature and then the other team member adding a feature.
