# GIT Y GITHUB :octocat:

_Getting started with Git and GitHub_

# GIT :octocat:
* [Read documentation](https://git-scm.com/)

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

### Example: Start a new repository local :zap:
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
```
```
git checkout master file.<ext>
```
<!-- ## Git reset vs. Git rm
- git rm --cached file.<ext> #staging -->

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

# GitHub :octocat:
* [Read documentation](https://docs.github.com/en/get-started/quickstart/hello-world)
* [Diagram Git and GitHub](https://static.platzi.com/media/public/uploads/git-github-17-28_e1ce4a1b-3b4c-4308-8057-b6c111ff7337.pdf)
<p align="center">
  <img src="/assets/img/git_github.png">
</p>

### Example: Contribute to an existing repository :zap:
```
# download a repository on GitHub to our machine
git clone https://github.com/name/repository.git

# change into the `repository` directory
cd repository

# create a new branch to store any new changes
git branch my-branch

# switch to that branch (line of development)
git checkout my-branch

# make changes, for example, edit `file1.md` and `file2.md` using the text editor

# stage the changed files
git add file1.md file2.md OR git add .

# take a snapshot of the staging area (anything that's been added)
git commit -m "description of changes"

# push changes to github
git push -u origin my-branch
```

### Example: Start a new repository and publish it to GitHub :zap:
```
# create a new directory, and initialize it with git-specific functions
mkdir my_folder
cd my_folder
git init

# create the first file in the project
touch README.md

# git isn't aware of the file, stage it
git add README.md

# take a snapshot of the staging area
git commit -m "add README to initial commit"

# provide the path for the repository you created on github
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY-NAME.git

# push changes to github
git push -u origin main
```

### Example: contribute to an existing branch on GitHub :zap:
```
# change into the `my_folder` directory
cd my_folder

# update all remote tracking branches, and the currently checked out branch
git pull

# change into the existing branch called `feature-a`
git checkout feature-a

# make changes, for example, edit `file1.md` using the text editor

# stage the changed file
git add file1.md

# take a snapshot of the staging area
git commit -m "edit file1"

# push changes to github
git push
```

## Models for collaborative development :boom:
There are two primary ways people collaborate on GitHub:
- Shared repository
- Fork and pull