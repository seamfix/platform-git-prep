# Key Git Concepts

Here are some some fundamental Git concepts that will help you navigate your workflow more efficiently.

## Staging

Staging is the process of selecting which changes you want to include in your next commit. Git allows you to stage individual files or all changes at once. When you stage changes, they are marked as "staged" in your Git status. You also have the option of using the source control panel on your VS code interface but learning the terminal code is important if you are running your code on a VM or only have access to a shell interface

**Tips:**

* Use `git add <file name>` to stage individual files.
* Use `git add .` to stage all changes in your current directory and subdirectories.
* Use `git reset <file name>` to unstage a specific file.

**Common mistakes:**

* Forgetting to stage changes before committing.
* Staging changes that shouldn't be committed (e.g. sensitive data).

**Useful commands:**

* `git status` to view which files are staged.
* `git diff --staged` to view the exact changes being staged.

## Branching

Branching is a way to isolate changes from the main codebase. It allows you to work on new features or bug fixes without affecting the main codebase.

**Tips:**

* Use `git branch <branch name>` to create a new branch.
* Use `git checkout <branch name>` to switch to a different branch.
* Use `git merge <branch name>` to merge changes from another branch.

**Common mistakes:**

* Forgetting to switch to the correct branch before making changes.
* Merging changes without resolving conflicts.

**Useful commands:**

* `git branch` to view all branches.
* `git log --graph` to view a visual representation of your commit history.

## Committing

Committing is the process of saving your changes to the local repository. Commits should be descriptive and contain a clear message explaining the changes made e.g feat: added bcrypt package.

**Tips:**

* Use `git commit -m "<commit message>"` to commit changes with a descriptive message.
* Use `git commit -a` to commit all changes in your current directory and subdirectories.
* Use `git commit --amend` to edit the most recent commit message.

**Common mistakes:**

* Not including a descriptive commit message.
* Committing sensitive data (e.g. passwords).

**Useful commands:**

* `git log` to view a list of all commits.
* `git show <commit hash>` to view the exact changes made in a specific commit.
* use a .gitignore file and a .env file to avoid pushing sensitive data to github.
* use a .env to house sensitive data like connection strings, passwords or api keys.

## Pushing and Pulling

Pushing is the process of uploading your local changes to a remote repository. Pulling is the process of downloading changes from a remote repository to your local machine.

**Tips:**

* Use `git push` to push your local changes to a remote repository.
* Use `git pull` to pull changes from a remote repository.

**Common mistakes:**

* Forgetting to pull changes before pushing.
* Pushing changes to the wrong branch.

**Useful commands:**

* `git remote -v` to view the URLs of your remote repositories.
* `git fetch` to download changes from a remote repository without merging.
