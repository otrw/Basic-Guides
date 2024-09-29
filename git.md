# Git Basics Cheatsheet

## Setting Up
- `git config --global user.name "Your Name"`: Set your name
- `git config --global user.email "your.email@example.com"`: Set your email

## Creating and Cloning Repositories
- `git init`: Initialize a new Git repository in the current directory
- `git clone <repository-url>`: Clone an existing repository

## Basic Workflow
- `git status`: Check the status of your working directory
- `git add <file>`: Add a file to the staging area
- `git add .`: Add all changed files to the staging area
- `git commit -m "Commit message"`: Commit staged changes with a message
- `git push`: Push commits to the remote repository
- `git pull`: Fetch and merge changes from the remote repository

## Branching
- `git branch`: List all local branches
- `git branch <branch-name>`: Create a new branch
- `git checkout <branch-name>`: Switch to a different branch
- `git checkout -b <branch-name>`: Create and switch to a new branch
- `git merge <branch-name>`: Merge a branch into the current branch

## Viewing Changes
- `git log`: View commit history
- `git diff`: View unstaged changes
- `git diff --staged`: View staged changes

## Undoing Changes
- `git restore <file>`: Discard changes in working directory
- `git restore --staged <file>`: Unstage a file
- `git reset HEAD~1`: Undo the last commit, keeping changes
- `git reset --hard HEAD~1`: Undo the last commit, discarding changes

## Remote Repositories
- `git remote add origin <repository-url>`: Add a remote repository
- `git remote -v`: List remote repositories
- `git fetch`: Download objects and refs from remote

## Help
- `git help <command>`: Get help for a specific Git command
-  [Generating a new SSH key and adding it to the ssh-agent](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
-  [Adding a new SSH key to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

<<<<<<< HEAD
Remember: Be careful with commands that discard changes (for example; `reset --hard`). If in doubt, make a backup or see if a safer alternative is available.
=======
#### Notes: 
- Be careful with commands that can discard changes (like `reset --hard`). 
- When in doubt, make a backup or use safer alternatives.
>>>>>>> 8d028e3 (minors updates to grammar & spelling)
