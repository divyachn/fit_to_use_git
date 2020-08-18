## Git Resources -

### Set up a repository

https://guides.github.com/introduction/git-handbook/

### Quick-start of git

https://git-scm.com/docs/gittutorial

### Play with branches

https://www.git-tower.com/learn/git/ebook/en/desktop-gui/advanced-topics/merge-conflicts#start \
https://www.git-tower.com/learn/git/faq/delete-local-branch

## Some commands I used frequently -

#### Command for cloning a repository in your local:
`git clone <git_URL> [Folder]` \
If you provide the name of Folder, the repository will be cloned inside it.

#### Check the branches (both remote and local):
`git branch -a`

#### Create a new branch but don't move to it:
`git branch <new_branch_name>`

#### Create a new branch and move to that branch:
`git checkout -b <new_branch_name>` \
**Note:** When you create a new banch (while you are on master), all changes in master are also included in `<new_branch>`.

#### Switch to a different branch:
`git checkout <branch_name>`

#### Pull any new changes made to remote into your local:
`git pull`

#### Check the status of local:
`git status`

#### In general when you make changes to local and want to push them to remote:
`git add <file_names_space_separated>` \
`git commit -m <small commit message>` \
`git push -u origin <remote_branch_name>` \
**Note:** *I prefer to have same name for both - remote and local branch*.

#### If you created a new local-branch and made some changes to it, use the following command to push this branch to remote:
`git push -u origin <branch_name>`

#### Pull a remote branch (test) not on local and move to that branch:
`git fetch origin test:test` \
`git checkout test`

#### Delete a branch on your local filesystem :
`git branch -d <branch_name>`

#### Delete the branch on remote:
`git branch -D <branch_name>`

#### Discard local changes and pull:
`git fetch --all` \
`git reset --hard origin <branch_name>`

#### Discard local changes that were not even added (using git add):
- Undo local changes for a single file: \
`git checkout -- <filename>`

- Undo all changes: \
`git reset --hard`
