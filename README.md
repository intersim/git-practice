# Git Practice

## Glossary
* repository
  * local
  * remote
* fork
  * upstream
* pull request

## Essential commands
* `git clone ${remote repo url}`
* `git add`
* `git commit`
* `git push`
* `git pull`
  * `git fetch`
  * `git merge`
* `git remote -v`
* `git remote add ${remote name} ${remote repo url}`
* `git remote remove ${remote name}`
* `git checkout -b ${new branch name}`
* `git checkout ${existing branch's name}`
* `git branch`

## Exercises
### Begin
1. A forks workshop on Github
1. A adds the original repo as a new remote called `upstream`
1. A adds B as collaborator on workshop on Github
1. A and B clone workshop onto their machine

### Without branching
_Bad in general, but sufficient for workshops_
1. A makes a commit and pushes it up to github
1. B pulls changes down from github, adds a commit, pushes it to github
1. A pulls changes down from github, adds a commit, pushes it to github
1. Rinse, repeat.

### With branching, but only one fork
_Better than above - good for senior phase projects!_
1. A makes a new branch
1. A makes a commit and pushes it to github
1. B fetches changes from github
1. B checkouts the new branch that A made
1. B adds a commit and pushes it to github
1. A pulls down changes from github, adds a commit, pushes it to github
1. B pulls down changes from github, adds a commit, pushes it to github
1. B makes a Pull Request on github (not the same thing as running git pull!)
1. A approves the request on github
1. A pulls down changes from the remote
1. Rinse, repeat.

### With branching and separate forks
[Reference gist by Omri](https://gist.github.com/omriBernstein/4fd2c21be8416d5e5a69aabc6fa94b82)

1. B forks workshop on Github
1. B adds the original repo as a new remote called `upstream`
1. B adds A's fork as another remote

