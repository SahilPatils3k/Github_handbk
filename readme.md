Here is your cleaned-up and properly formatted `README.md` file for your **GitHub Basics Session**:

---

````markdown
# GitHub Basics: Session Guide

Welcome to the **GitHub Basics** session!  
This guide will help you understand how to clone a repository, push and pull code, and work with branches using Git and GitHub. Follow along during the session and use this as a reference.

---

## 📘 What You'll Learn

- **Git**: A tool to track code changes and collaborate.
- **GitHub**: A platform to host and share Git repositories.

### 🔑 Key Terms

| Term        | Description |
|-------------|-------------|
| **Repository (Repo)** | A project folder with your files and history. |
| **Clone**    | Copy a repo from GitHub to your computer. |
| **Commit**   | Save changes locally with a message. |
| **Push**     | Upload local changes to GitHub. |
| **Pull**     | Download updates from GitHub. |
| **Branch**   | A separate version of your repo for new features or fixes. |

---

## ⚙️ Prerequisites

1. **Install Git**  
   [Download Git](https://git-scm.com)

2. **Check Git Installation**
   ```bash
   git --version
````

3. **Set Up Git Config**

   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   ```

---

## 🔽 1. Cloning a Repository

Clone this repository to your computer:

```bash
git clone https://github.com/username/repository-name.git
cd repository-name
```

* Replace the URL with your actual repository link from GitHub.
* This downloads the project and navigates into its folder.

---

## 📝 2. Making and Committing Changes

Make changes to any file, then run:

```bash
git status
```

* Shows modified/untracked files.

```bash
git add .
```

* Stages all changes. Use `git add filename` to stage specific files.

```bash
git commit -m "Describe your changes"
```

* Saves changes locally with a commit message.

---

## 🚀 3. Pushing to GitHub

Send local commits to GitHub:

```bash
git push origin main
```

* Replace `main` with your branch name if different.

---

## ⬇️ 4. Pulling from GitHub

Get the latest updates from GitHub:

```bash
git pull origin main
```

* This fetches and merges changes into your local branch.

---

## 🌿 5. Working with Branches

Branches let you work independently on new features.

```bash
git branch
```

* Lists local branches (`*` shows the current one).

```bash
git checkout -b feature-name
```

* Creates and switches to a new branch (e.g., `add-feature`).

```bash
git push origin feature-name
```

* Pushes the new branch to GitHub.

### 🔀 Merging Branches

```bash
git checkout main
git pull origin main
git merge feature-name
git push origin main
```

### 🗑️ Deleting a Branch

```bash
git branch -d feature-name
```

* Deletes the branch locally after merge.

---

## 🧪 Example Workflow

```bash
git clone https://github.com/username/repository-name.git
cd repository-name
git checkout -b my-feature
# Edit files
git add .
git commit -m "Added my feature"
git push origin my-feature
git checkout main
git pull origin main
git merge my-feature
git push origin main
git branch -d my-feature
```

---

## ✅ Practice Task

1. Clone this repo.
2. Create a branch named `yourname-update` (e.g., `john-update`).
3. Edit this README (add your name below).
4. Commit and push to your branch.
5. Share your branch name with the instructor.

### Add Your Name Here:

* \[Your Name]

---

## 🛠️ Troubleshooting

* **Authentication Error**:
  Ensure you have GitHub credentials or SSH keys set up. See [GitHub Docs](https://docs.github.com/en).

* **Merge Conflicts**:
  If changes overlap, manually edit the files, then:

  ```bash
  git add .
  git commit -m "Resolved conflicts"
  git push
  ```

---

## 📚 Resources

* [GitHub Docs](https://docs.github.com/)
* [Git Cheat Sheet (PDF)](https://education.github.com/git-cheat-sheet-education.pdf)

---

Happy Coding! 🚀

```

---

### ✅ How to Use:
- Save this as `README.md` in your GitHub repo.
- Let participants follow along.
- Ask them to **edit the README** and **push their changes** as a practice task.

Would you also like a simple slide deck for presenting this?
```
