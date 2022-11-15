# Version Control w/ Git

Git is a very powerful protocol that is widely used for controlling the versions of a repo. With this tutorial you'll learn to use Git.

## Installing Git
first, you'll need to check if `git` is already installed in your system (it usually comes by default in most mac and linux machines).

```
# Checking if git is installed
git version
```

If `git` is installed the output should be something like this
```
git version 2.37.1 
```

If `git` is not installed you can check the official installation guide. [[Install git]](https://github.com/git-guides/install-git) 

## Getting Started

After installing `git` in your system you'll need to make a few configurations.

The first thing is to setup an username and email address.
```
git config --global user.name <username>  # To setup username
git config --global user.email <example@email.com>  # To setup email
```

To list all your current configurations use.
```
git config --list
```
## Local Version Control
With Git it's possible to transform a local directory into a Git repository. To do this we first need to `cd` into the directory repo and initialize it with Git.
```
cd <repository_path>
git init
```
This command will create a subdirectory called .git that contains all the necessary files from your repository.

After initializing the directory, we can use the `status` command, which will be very useful to keep track of every step.
```
git status
```

The output should be something like this
```
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)
```

To begin with version control you'll need to make an initial **commit**. 

In order to do this you'll need to specify which file, or files, to version control.
```
git add file
git status
```

Step 1. git clone

cd to cloned repo

git status // verify status

git add <file> // make changes

git commit // makes changes on local repo (main) and adds description to new added file

s
INSERT mode
first commit
description

esc + :wq

git push // adds changes to GitHub repo (origin)

git log // shows each commit

git log --oneline // Shows each commit and hash

git branch -avv // verifica branch

git checkout <hash> ir para uma branch

git checkout main // volta para main


