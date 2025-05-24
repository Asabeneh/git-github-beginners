# Git and GitHub for Beginners

## Git

Expanded Git Refresher Guide
This guide provides essential Git commands for managing your project, from initialization to collaboration and history management.
Initialize and Check Status

git initInitializes a new Git repository in the current directory.
git statusDisplays the current state of the working directory and staging area, showing modified, staged, and untracked files.
git logShows the commit history for the current branch.

Staging and Committing Changes

git add <filename>Adds a specific file to the staging area for the next commit.
git add .Adds all modified and new files in the current directory to the staging area.
git commit -m "commit message"Commits staged changes with a descriptive message.
git commit --amendModifies the most recent commit (e.g., to edit the commit message or add more changes).

Remote Repository

git remote add origin <url_of_remote_repo>Links the local repository to a remote repository (e.g., GitHub, GitLab).
git push -u origin <branch>Pushes the specified branch (e.g., master or new-branch) to the remote repository and sets it as the upstream branch.
git pull origin <branch>Fetches and merges changes from the specified remote branch into the current branch.
git clone <url_of_remote_repo>Downloads a repository from a remote URL to your local machine.

Branching

git branch <new-branch>Creates a new branch named <new-branch>.
git checkout <new-branch>Switches to the specified branch.
git checkout -b <new-branch>Creates and immediately switches to a new branch.
git branchLists all branches in the repository, with the current branch marked by an asterisk.
git merge <branch>Merges the specified branch into the current branch.
git branch -d <branch>Deletes the specified branch (if fully merged).

Undoing Changes

git reset <filename>Unstages a file from the staging area but preserves changes in the working directory.
git checkout -- <filename>Discards changes to a file in the working directory, reverting it to the last committed state.
git revert <commit>Creates a new commit that undoes the changes from a specified commit.

Collaboration

git fetch originRetrieves updates from the remote repository without merging them.
git remote -vLists all remote repositories and their URLs.
git stashTemporarily saves uncommitted changes, allowing you to switch branches.
git stash popRestores the most recently stashed changes and removes them from the stash.



## Demo

[live](https://github.com/Asabeneh/git-github-beginners)
