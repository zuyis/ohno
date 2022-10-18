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

### big no-no's
- committing passwords!!!!!!!

### typical commands
set remote

 `git clone `

 `git fetch`

 `git checkout [-b] branchname`
 
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
