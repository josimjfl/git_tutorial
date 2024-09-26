# Git Tutorial: 
## by JFL IT Lab
### jflitlab@gmail.com
#### Josim JFL
---
Git on both the Desktop (with GitHub Desktop) and Online (via GitHub, GitLab, etc.) with command line commands (CMD):
# Git Tutorial: Desktop and Command Line

## Table of Contents
1. [Introduction to Git](#introduction-to-git)
2. [GitHub Desktop Setup](#github-desktop-setup)
    - Install GitHub Desktop
    - Cloning a Repository
    - Committing and Pushing Changes
3. [Git via Command Line](#git-via-command-line)
    - Install Git
    - Basic Git Commands
    - Workflow Example with Command Line
4. [Working with Git Remotely (GitHub)](#working-with-git-remotely)
    - Push Local Repos to GitHub
    - Cloning Repositories from GitHub
5. [Syncing GitHub Desktop and Command Line](#syncing-github-desktop-and-command-line)

---

## Introduction to Git

Git is a version control system that allows multiple developers to work on a project simultaneously and track changes in the source code. Git is popular for collaboration and is often used with platforms like GitHub, GitLab, and Bitbucket.

---

## GitHub Desktop Setup

GitHub Desktop is a GUI tool that simplifies Git version control without requiring command line usage. Here’s how to get started:

### 1. **Install GitHub Desktop**
- Download and install GitHub Desktop from the official site: [GitHub Desktop](https://desktop.github.com/)
  
### 2. **Cloning a Repository**
1. Open GitHub Desktop.
2. Click `File > Clone repository`.
3. Enter the repository URL or select one from your GitHub account.
4. Choose a local path and click `Clone`.

### 3. **Committing and Pushing Changes**
1. **Making Changes**: Modify files in your local repository.
2. **Stage and Commit**: Go back to GitHub Desktop. You will see your changes. Add a commit message and click `Commit to main`.
3. **Push Changes**: After committing, click `Push origin` to sync your local changes with the remote repository.

---

## Git via Command Line

If you prefer to use the command line for more granular control, here’s how to do it.

### 1. **Install Git**
- Download and install Git from [git-scm.com](https://git-scm.com/).
- Verify installation:
  ```bash
  git --version
  ```

### 2. **Basic Git Commands**
- **Initialize a repository**:
  ```bash
  git init
  ```
- **Clone a remote repository**:
  ```bash
  git clone <repository-url>
  ```
- **Check repository status**:
  ```bash
  git status
  ```
- **Stage changes**:
  ```bash
  git add .
  ```
- **Commit changes**:
  ```bash
  git commit -m "Your commit message"
  ```
- **Push changes to remote**:
  ```bash
  git push origin main
  ```

### 3. **Workflow Example with Command Line**
1. **Create a new local repository**:
   ```bash
   mkdir my_project
   cd my_project
   git init
   ```
2. **Stage and commit changes**:
   ```bash
   git add .
   git commit -m "Initial commit"
   ```
3. **Link to GitHub and push**:
   ```bash
   git remote add origin <repository-url>
   git branch -M main
   git push -u origin main
   ```

---

## Working with Git Remotely (GitHub)

To work with GitHub and Git on the command line, you need to push and pull code between your local machine and GitHub.

### 1. **Push Local Repos to GitHub**
1. Create a new repository on GitHub without a README (so it’s empty).
2. Link your local repository:
   ```bash
   git remote add origin https://github.com/yourusername/your-repo.git
   ```
3. Push the repository:
   ```bash
   git push -u origin main
   ```

### 2. **Cloning Repositories from GitHub**
If you want to work on an existing project:
```bash
git clone https://github.com/yourusername/your-repo.git
```

---

## Syncing GitHub Desktop and Command Line

If you switch between GitHub Desktop and the command line, Git keeps everything synced.

### 1. **Making Changes in GitHub Desktop**
- Commit and push changes from GitHub Desktop.
- Open the terminal in the same repository:
  ```bash
  git pull origin main  # Sync changes from remote to your local terminal session
  ```

### 2. **Making Changes in Command Line**
- Make changes, commit, and push via command line:
  ```bash
  git add .
  git commit -m "Updated some files"
  git push origin main
  ```
- Open GitHub Desktop, and your changes will be reflected there automatically.

---

### Conclusion

You can easily manage repositories with both GitHub Desktop and Git via the command line. Use the tool that best suits your workflow—GUI for simplicity or command line for more flexibility. You can sync both methods seamlessly and collaborate with others using GitHub.
