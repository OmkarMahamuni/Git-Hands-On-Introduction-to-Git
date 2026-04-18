## Setup & Config

* **`git config --global user.name "Name"`**: Sets the author name attached to your commits.
  * *Example:* `git config --global user.name "Omkar"`
* **`git config --global user.email "Email"`**: Sets the author email attached to your commits.
  * *Example:* `git config --global user.email "omkar@example.com"`
* **`git init`**: Start new Git repo in the directory that you run this command.
  * *Example:* `git init`

## Basic Workflow

* **`git status`**: Shows the current state of your working directory and staging area (tells you what has changed).
  * *Example:* `git status`
* **`git add <file>` / `git add . `**: Moves a changed file into the Staging Area, getting it ready to be committed.
  * *Example:* `git add git-commands.md` and `git add .` to add everything.
* **`git commit -m "Message"`**: Permanently saves the staged changes into the local repository's history.
  * *Example:* `git commit -m "Added a new feature"`

## Viewing Changes

* **`git log` / `git log --oneline`**: Shows the complete history of all commits in the repository.
  * *Example:* `git log` or `git log --oneline` for a one line compact view.
* **`git diff`**: Shows the exact lines of code that were added or deleted since the last commit.
  * *Example:* `git diff`

## Commit no 2

* This is commit no 2

# Branching & Merging
* **`git branch`**: Lists all the branches in your local repository. The current branch is highlighted with a `*`.
  * *Example:* `git branch`
* **`git branch <name>`**: Creates a new branch but does *not* switch to it.
  * *Example:* `git branch feature-login`
* **`git switch <name>`**: Moves your working directory to the specified branch. (This is the modern, safer alternative to `git checkout`).
  * *Example:* `git switch feature-login`
* **`git switch -c <name>`**: Creates a new branch AND switches to it in one single command.
  * *Example:* `git switch -c bugfix-header`
* **`git branch -d <name>`**: Safely deletes a branch (only if it has been merged). Use `-D` to force delete an unmerged branch.
  * *Example:* `git branch -d feature-2`

## Remote Repositories (GitHub)
* **`git remote add origin <url>`**: Connects your local repository to a remote server (like GitHub). "Origin" is just the default nickname for that server.
* **`git push -u origin <branch>`**: Uploads your local branch commits to the remote server. The `-u` flag links your local branch to the remote branch so future pushes just require typing `git push`.
  * *Example:* `git push -u origin main`
* **`git pull`**: Downloads changes from the remote repository and immediately merges them into your current local branch.

