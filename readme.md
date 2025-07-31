GitHub Session Handbook: Getting Started with Git and GitHub
This handbook covers the basics of using Git and GitHub, including cloning a repository, pushing and pulling code, key terminologies, and working with branches. Each command is explained clearly for beginners.
1. Introduction to Git and GitHub

Git: A version control system that tracks changes in your code and allows multiple people to collaborate.
GitHub: A platform for hosting Git repositories online, enabling collaboration and code sharing.
Repository (Repo): A folder/project containing your files and their version history.
Clone: Downloading a copy of a repository to your local machine.
Commit: Saving changes to your local repository with a descriptive message.
Push: Uploading your local changes to the remote repository on GitHub.
Pull: Downloading updates from the remote repository to your local machine.
Branch: A parallel version of your repository, allowing you to work on features or fixes separately.

2. Setting Up Git
Before starting, ensure Git is installed on your machine.
Command: Check Git Installation
git --version


Explanation: Displays the installed Git version (e.g., git version 2.39.2). If not installed, download Git from git-scm.com.

Command: Configure Git
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"


Explanation: Sets your name and email for commit messages, associating your identity with changes.

3. Cloning a Repository
Cloning copies a GitHub repository to your local machine.
Command: Clone a Repository
git clone https://github.com/username/repository-name.git


Explanation: Downloads the repository to a folder named repository-name. Replace the URL with the repository’s HTTPS link (found on GitHub under the "Code" button).
Example: git clone https://github.com/johndoe/my-project.git creates a my-project folder with the repo’s contents.

Command: Navigate to Repository
cd repository-name


Explanation: Changes your terminal’s working directory to the cloned repository folder (e.g., cd my-project).

4. Making Changes and Committing
After modifying files, you save changes locally using commits.
Command: Check Status
git status


Explanation: Shows the current state of your repository, listing modified, staged, or untracked files.

Command: Stage Changes
git add .


Explanation: Stages all modified/new files for the next commit. Use git add filename to stage specific files.

Command: Commit Changes
git commit -m "Descriptive message"


Explanation: Saves staged changes locally with a message describing the changes (e.g., git commit -m "Added homepage").

5. Pushing Changes to GitHub
Pushing uploads your local commits to the remote repository.
Command: Push Changes
git push origin main


Explanation: Sends your local commits to the main branch on the remote repository (origin is the default name for the remote). Replace main with your branch name if different (e.g., master).

6. Pulling Changes from GitHub
Pulling downloads updates from the remote repository to your local machine.
Command: Pull Changes
git pull origin main


Explanation: Fetches and merges changes from the main branch of the remote repository into your local branch. Ensures your local repo is up-to-date.

7. Working with Branches
Branches allow you to work on features or fixes without affecting the main codebase.
Command: List Branches
git branch


Explanation: Displays all local branches, with an asterisk (*) indicating the current branch.

Command: Create a Branch
git branch feature-name


Explanation: Creates a new branch named feature-name (e.g., git branch add-login).

Command: Switch to a Branch
git checkout feature-name


Explanation: Switches your working directory to the feature-name branch (e.g., git checkout add-login).

Command: Create and Switch Branch (Shortcut)
git checkout -b feature-name


Explanation: Combines creating and switching to a new branch in one command (e.g., git checkout -b add-login).

Command: Push a Branch to GitHub
git push origin feature-name


Explanation: Uploads the feature-name branch to the remote repository.

Command: Merge a Branch
git checkout main
git merge feature-name


Explanation: Merges changes from feature-name into the main branch. Run these commands after switching to main.

Command: Delete a Branch
git branch -d feature-name


Explanation: Deletes the feature-name branch locally after merging. Use -D instead of -d to force deletion without merging.

8. Basic Workflow Example

Clone the repo: git clone https://github.com/username/repo.git
Navigate: cd repo
Create a branch: git checkout -b new-feature
Make changes to files.
Stage changes: git add .
Commit: git commit -m "Added new feature"
Push branch: git push origin new-feature
Switch to main: git checkout main
Pull updates: git pull origin main
Merge branch: git merge new-feature
Push to main: git push origin main
Delete branch: git branch -d new-feature

9. Tips for the Session

Demonstrate Live: Use a sample repository on GitHub to show cloning, committing, pushing, pulling, and branching.
Explain Errors: Common issues include:
Authentication: Ensure users have GitHub credentials or SSH keys set up.
Merge Conflicts: Explain they occur when changes overlap; resolve by editing conflicting files and committing.


Practice: Let attendees clone a repo, make a small change (e.g., edit a README), and push to a branch.
Resources: Recommend GitHub Docs and Git Cheat Sheet.
