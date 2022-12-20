# Git Version Control

Git is a popular version control system that is used by developers and organizations to manage and track changes to their code and projects. It allows multiple users to collaborate on a project, and provides a history of the changes and modifications that have been made to the code.

In this tutorial, I will explain how to use Git to create a new repository, make changes to files in the repository, and share those changes with others.

# Getting Started
To use Git, you will need to install it on your computer, and create a Git repository for your project. A Git repository is a local directory that contains the code and files for your project, and tracks the changes and modifications that have been made to the code.

### Installing Git
To install Git on your computer, you can follow these steps:

1. Download the latest version of Git from the Git website.
2. Follow the instructions to install Git on your computer.
3. Open a terminal or command prompt, and verify that Git is installed and working by running the following command:
```
git --version
```

After installing `git` in your system you'll need to make a few configurations.

The first thing is to setup an username and email address.
```
git config --global user.name <username>  # To setup username
git config --global user.email <example@email.com>  # To setup email
```

## Creating a Git Repository
To create a new Git repository, you first need to create a new directory for your project. This can be done using the `mkdir` command in your terminal or command prompt. For example:
```
mkdir my-project
```

Once you have created your project directory, you can move into it using the `cd` command. For example:
```
cd <repository_path>
```

To initialize your Git repository, you can use the `git init` command. This will create a new `.git` directory inside your project directory, which will store all of the information about your project's history.

```
git init
```

### Adding Files to the Repository
Once you have initialized your Git repository, you can start adding files to it. This can be done using the `git add` command, followed by the name of the file you want to add. For example:
```
git add myfile.txt
```

You can also add all of the files in your project directory at once using the `git add .` command. This will add all of the files, including any new files that you may have created since initializing your repository.

```
git add .
```
### Commiting Changes
Once you have added your files to the Git repository, you can commit your changes. A commit is a snapshot of your project at a specific point in time. When you make a commit, you include a message that describes the changes you have made.

To make a commit, you can use the `git commit` command, followed by the `-m` option and a message describing your changes. For example:
```
git commit -m "Added myfile.txt to the repository"
```

## Sharing Changes with Others
Once you have made some commits to your Git repository, you may want to share your changes with others. This can be done using a remote repository, which is a Git repository that is hosted on a server and can be accessed by multiple people.

To push your changes to a remote repository, you first need to add the remote repository to your local repository using the `git remote add` command. This command takes two arguments: the name you want to give the remote repository, and the URL of the remote repository. For example:

```
git remote add origin https://github.com/username/my-project.git
```

Once you have added the remote repository, you can push your changes to it using the `git push` command. This command takes two arguments: the name of the remote repository, and the name of the branch you want to push your changes to. For example:
```
git push origin master
```

This will push your local changes to the `master` branch of the remote repository, which is the main branch of the project.

## Managing Versions

In Git, you can use the `git log` command to view the history of your repository. This command will show a list of all of the commits that have been made to your repository, along with the commit messages and the date and time of each commit.

To view the history of your repository, you can use the `git log` command with the `--oneline` and `--decorate` options. For example:
```
git log --oneline --decorate
```

This will show the commit history in a condensed format, with each commit on a separate line and the branch and tag names displayed next to each commit.

To view the details of a specific commit, you can use the `git show` command followed by the commit hash. The commit hash is a unique identifier for each commit in your repository, and you can find it by looking at the output of the `git log` command. For example:
```
git show abc123
```

This will show the details of the commit with the hash `abc123`, including the changes that were made in that commit and the commit message.

To revert to a previous version of your repository, you can use the `git checkout` command followed by the commit hash. This will move your repository to the state it was in at the time of that commit. For example:
```
git checkout abc123
```
This will move your repository to the state it was in at the time of the commit with the hash `abc123`. Keep in mind that this will discard any changes that have been made since that commit, so it should be used with caution.

In summary, you can use the `git log` command to view the history of your repository, the `git show` command to view the details of a specific commit, and the `git checkout` command to move your repository to a previous version.


