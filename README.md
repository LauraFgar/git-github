## INSTALL
- https://git-scm.com/ 

## Config git
- git config --list
- git config --global user.name = "Your name" 
- git config --global user.email = "Your email" 

## Status Git
- 1: Working directory (untracked)
- 2: Staging directory (tracked)
- 3: Repository (IDCommit1)

## Comands basic git
Initialize a repository from an existing directory
- git init
- git status
- (git add file.<ext>) OR (git add .) #staging
- git commit -m "This is message" #repository

<!-- ## Analyze changes git
- git show
- git log file.<ext>
- git diff IDCommit1 IDCommit2 

## Git reset vs. Git rm
- git rm --cached file.<ext> -->


## Branchs
- GitFlow: Simple pattern to branch (Patrón simple para ramificar)
    https://www.campingcoder.com/2018/04/how-to-use-git-flow/
    https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow

- git branch
- git branch your_name_branch_here
- git checkout your_name_branch_here