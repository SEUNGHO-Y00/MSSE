#  Introduction to Git and GitHub

1. Motivation

2. Git

* Installation and VS Code
  - open WSL terminal
  - install Git
  - confirm your password
  - check version = git --version
  - configure git = git config --global user.name seungho / git config --global user.email seungho.yoo@berkeley.edu
    - git has three levels of access (local, global, system)
  - check config = git config --list
  - Git and VS Code

* Status, add and commit

working directory | staging area | local repo |
|:--:|:--:|:--:|
modify & safe the file |  |
git status|  | -> git commit
|  | -> git add |
git restore --staged <- |  | git status

* Compare differences

1) A new file (--.py) in the working directory = git status, git add, git status
2) We kept working on the file and have two versions now!
   - before adding or committing to the repo -> review changes!

* restoring from index, stage and commit

1) changing file in working directory = undo:git restore
2) git add file from working directory to stage area = undo:gitrestore --staged
   - git restore --source=HEAD~X
   - git restore --staged
   - git restore

3. GitHub

* Create your repo

1) got to github.com = register and confirm email address
2) create new repository = Dashboard

* invite a coworker

1) go to setting
2) go to collaborators = add member

* push

  - clone the repo:
1) git clone address

  - push the change
1) git add
2) git commit -m "my message"
3) git push address.git main

* fetch, merge, pull

  - git fetch
  - git merge
    - does update your working directory
  - git pull
    - 
