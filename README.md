# GIT Y GITHUB :octocat:

_Getting started with Git and GitHub_

## Install GIT :checkered_flag:
```
https://git-scm.com/ 
```

## Configuration :wrench:
```
git config --list
```
```
git config --global user.name = "Your name" 
```
```
git config --global user.email = "Your email" 
```

## Workflow local :house:
- Working directory (untracked)
- Staging directory (tracked)
- Repository (IDCommit)

<p align="center">
  <img src="/assets/img/workflow.png">
</p>

## Basic commands :walking:
```
git init
```
```
git clone
```
```
git add
```
```
git commit
```
```
git status
```
```
git branch
```
```
git merge
```
```
git pull
```
```
git push
```

### Example: Start a new repository local :sunglasses:
```
mkdir test
cd test
touch test.py
ls
git init
ls -al
git status
git add test.py
git rm --cached test.py
git commit -m "description of changes"
--repeat
```

## Analyze changes
```
git show file.<ext>
```
```
git log file.<ext>
```
```
git diff <IDCommit1> <IDCommit2>
```

## Back to the past
```
git checkout IDCommit1 file.<ext>
git checkout master file.<ext>
```
<!-- ## Git reset vs. Git rm
- git rm --cached file.<ext> #staging -->

## GitHub
* [Read documentation](https://docs.github.com/en/get-started/quickstart/hello-world)

### Example: Contribute to an existing repository :sunglasses:
```
# download a repository on GitHub to our machine
# Replace `owner/repo` with the owner and name of the repository to clone
git clone https://github.com/owner/repo.git

# change into the `repo` directory
cd repo

# create a new branch to store any new changes
git branch my-branch

# switch to that branch (line of development)
git checkout my-branch

# make changes, for example, edit `file1.md` and `file2.md` using the text editor

# stage the changed files
git add file1.md file2.md

# take a snapshot of the staging area (anything that's been added)
git commit -m "my snapshot"

# push changes to github
git push --set-upstream origin my-branch
```
## Branchs
* [GitFlow](https://www.campingcoder.com/2018/04/how-to-use-git-flow/) - Simple pattern to branch (Patrón simple para ramificar)

<p align="center">
  <img src="/assets/img/gitflow-diagram.jpg">
</p>

```
git branch
git branch your_name_branch_here
git checkout your_name_branch_here

OR

git checkout -b your_name_branch_here
```