## Git for BI

This is an introduction to using Git, additional information can be found by googling.
The goal is for our team to have a central repository for code and knowledge sharing, especially SQL queries. 

### Set up
- get added to Alaska org in Github
- https://git-scm.com/downloads
- set up ssh: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent


### best practices
- commit at regularly at appropriate times and use clear commit messages
- pull request must be reviewed by another person before merging
- always include a readme.md

### DO NOT DO THIS
don't commit any passwords!!!!!!!

### for existing repositories
start by cloning the repo\
`git clone existing-repo-url`

you have the option to create your own branch\
`git checkout [-b] branchname`

or you can check out an existing branch\
`git fetch`\
`git branch -a -v`\
`git switch remote-branch-name`

if you forget to do either and started making changes off main, you can switch to a different/new branch\
`git switch -c new-local-branch-name`\
or\
`git switch existing-branch-name`

to merge changes from a different branch into your branch\
`git merge other-branch-name`

### after you make changes

```
git add .
git commit -m 'something helpful for others'
git push origin your-branch-name

```

### if you mess up
reset to the most recent commit, with your changes\
`git reset`\
undo 1 commit and keep track of the undo\
`git revert HEAD~1`\
nuclear option to erase everything and restart for the repo\
`git reset --hard`

### creating a repository
1. create a repo on github. select add a `README.md` and `.gitignore` files
2. follow the code below or what is on github

``` 
git init
git add README.md
git add .gitignore
git commit -m "first commit"
git branch -M main
git remote add origin url-to-your-repo
git push -u origin main
```
