# Version Control w/ Git

Git is a very powerful protocol that is widely used for controlling the versions of a repo. With this tutorial you'll learn to use Git.

## Installing Git
first, you'll need to check if `git` is already installed in your system (it usually comes by default in most mac and linux machines).

```
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

To list all current configurations use the following command.
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

Now let's add a `README.txt` file to the repository and repeat the `git status` command.
<img width="794" alt="Screenshot 2022-11-18 at 23 42 14" src="https://user-images.githubusercontent.com/104539928/202830565-50a996fa-461a-4c53-a985-ee53a373532c.png">

The output should be something like this
```
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	README.txt

nothing added to commit but untracked files present (use "git add" to track)
```
The `git status` command will keep track of all untracked and tracked files

To begin with version control we need to make an initial **commit**. To do this, we need to specify which file, or files, to version control.
```
git add README.txt
git status
```

The output should be something like this
```
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   README.txt

```
Now the `README.txt` file was added for version control. To save or `commit` changes we use the `git commit` command.

```
git commit
```

you'll be asked to enter a small text specifying all the changes.

if you are using `vim`, to start writing you'll first press the `s` key, to save the text press `esc` key followed by `:wq`

<img width="794" alt="Screenshot 2022-11-19 at 00 04 33" src="https://user-images.githubusercontent.com/104539928/202831249-45838109-97b4-4d7a-99b2-9d5106d4918a.png">


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


