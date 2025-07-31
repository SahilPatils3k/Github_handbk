GitHub Basics: Session Guide
Welcome to the GitHub Basics session! This README provides a quick guide to cloning a repository, pushing and pulling code, and working with branches using Git and GitHub. Follow along during the session and use this as a reference.
What You'll Learn

Git: A tool to track code changes and collaborate.
GitHub: A platform to host and share Git repositories.
Key Terms:
Repository (Repo): A project folder with your files and their history.
Clone: Copy a repo from GitHub to your computer.
Commit: Save changes locally with a message.
Push: Upload local changes to GitHub.
Pull: Download updates from GitHub to your computer.
Branch: A separate version of your repo for new features or fixes.



Prerequisites

Install Git: Download from git-scm.com.
Check installation: Run git --version in your terminal.
Set up Git:git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

Sets your name and email for commits.

1. Cloning a Repository
Clone this repository to your computer to get started.
git clone https://github.com/username/repository-name.git

Downloads the repo to a folder named repository-name. Replace the URL with this repo’s link (find it under the "Code" button on GitHub).
cd repository-name

Moves into the repo’s folder.
2. Making and Committing Changes
Edit files and save changes locally.
git status

Shows modified or untracked files.
git add .

Stages all changed files for committing. Use git add filename for specific files.
git commit -m "Describe your changes"

Saves staged changes with a message (e.g., git commit -m "Updated README").
3. Pushing to GitHub
Upload your changes to GitHub.
git push origin main

Sends local commits to the main branch on GitHub. Replace main with your branch if different.
4. Pulling from GitHub
Download updates from GitHub.
git pull origin main

Fetches and merges changes from the main branch on GitHub to your local repo.
5. Working with Branches
Branches let you work on features without affecting the main code.
git branch

Lists all local branches, with * showing the current branch.
git checkout -b feature-name

Creates and switches to a new branch (e.g., git checkout -b add-feature).
git push origin feature-name

Uploads the branch to GitHub.
git checkout main
git merge feature-name

Switches to main and merges feature-name into it.
git branch -d feature-name

Deletes the branch locally after merging.
Example Workflow

Clone: git clone https://github.com/username/repository-name.git
Navigate: cd repository-name
Create branch: git checkout -b my-feature
Edit files (e.g., this README).
Stage: git add .
Commit: git commit -m "Added my feature"
Push: git push origin my-feature
Switch to main: git checkout main
Pull updates: git pull origin main
Merge: git merge my-feature
Push to main: git push origin main
Delete branch: git branch -d my-feature

Practice Task

Clone this repo.
Create a branch named yourname-update (e.g., john-update).
Edit this README (add your name below).
Commit and push to your branch.
Share your branch name with the instructor.

Add Your Name Here:

[Your Name]

Troubleshooting

Authentication Error: Ensure you have GitHub credentials or SSH keys set up. Check GitHub Docs.
Merge Conflicts: If changes overlap, edit the conflicting files, then run git add, git commit, and git push.

Resources

GitHub Docs
Git Cheat Sheet

Happy coding!