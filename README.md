# Git and GitHub for Beginners

## Git Introduction

This guide covers essential Git commands for managing your project, from initialization to collaboration, history management, and more. All commands are formatted for use in a terminal.

## Initialize and Check Status

- `git init`  
  Initializes a new Git repository in the current directory, creating a `.git` folder.
- `git status`  
  Shows the current state of the working directory and staging area, listing modified, staged, and untracked files.
- `git log`  
  Displays the commit history for the current branch, including commit hashes, authors, and messages.
- `git log --oneline`  
  Shows a compact, one-line summary of the commit history.

## Staging and Committing Changes

- `git add <filename>`  
  Adds a specific file to the staging area for the next commit.
- `git add .`  
  Adds all modified and new files in the current directory to the staging area.
- `git commit -m "commit message"`  
  Commits staged changes with a descriptive message.
- `git commit --amend`  
  Modifies the most recent commit, allowing changes to the commit message or staged files.

## Viewing Differences

- `git diff`  
  Shows changes between the working directory and the staging area.
- `git diff --staged`  
  Displays changes in the staging area compared to the last commit.

## Remote Repository

- `git remote add origin <url_of_remote_repo>`  
  Links the local repository to a remote repository (e.g., GitHub, GitLab).
- `git push -u origin <branch>`  
  Pushes the specified branch (e.g., `master` or `new-branch`) to the remote repository and sets it as the upstream branch.
- `git pull origin <branch>`  
  Fetches and merges changes from the specified remote branch into the current branch.
- `git clone <url_of_remote_repo>`  
  Downloads a repository from a remote URL to your local machine.
- `git fetch origin`  
  Retrieves updates from the remote repository without merging them.
- `git remote -v`  
  Lists all remote repositories and their URLs.

## Branching

- `git branch <new-branch>`  
  Creates a new branch named `<new-branch>`.
- `git checkout <new-branch>`  
  Switches to the specified branch.
- `git checkout -b <new-branch>`  
  Creates and immediately switches to a new branch.
- `git branch`  
  Lists all branches in the repository, with the current branch marked by an asterisk.
- `git merge <branch>`  
  Merges the specified branch into the current branch.
- `git branch -d <branch>`  
  Deletes the specified branch (if fully merged).

## Undoing Changes

- `git reset <filename>`  
  Unstages a file from the staging area but preserves changes in the working directory.
- `git checkout -- <filename>`  
  Discards changes to a file in the working directory, reverting it to the last committed state.
- `git revert <commit>`  
  Creates a new commit that undoes the changes from a specified commit.
- `git reset --hard <commit>`  
  Resets the working directory and index to a specified commit, discarding all changes.

## Stashing Changes

- `git stash`  
  Temporarily saves uncommitted changes, allowing you to switch branches.
- `git stash pop`  
  Restores the most recently stashed changes and removes them from the stash.
- `git stash list`  
  Lists all stashed changesets.

## Tagging

- `git tag <tagname>`  
  Creates a lightweight tag at the current commit.
- `git tag -a <tagname> -m "tag message"`  
  Creates an annotated tag with a message.
- `git push origin <tagname>`  
  Pushes a specific tag to the remote repository.

## Tips

- Always use clear, descriptive commit messages to document changes.
- Run `git status` frequently to understand the state of your repository.
- Use `git diff` to review changes before staging or committing.
- Be cautious with commands like `git reset --hard`, as they can permanently discard changes.

This guide is a quick reference for common Git workflows. For more details, consult the official Git documentation (`git --help` or `man git`).

## Demo

[live](https://github.com/Asabeneh/git-github-beginners)
