# Local Machine to GitHub Repository
A project that demonstrates how to move source code from a local machine to a GitHub repository using Git version control.

### Overview
Version control is a fundamental skill for developers, DevOps engineers, and cloud professionals. This project provides a practical introduction to Git and GitHub by walking through the complete workflow of creating a local repository, tracking changes, creating commits, connecting to GitHub, and pushing code to a remote repository.

By following this project, you will learn how Git enables efficient source code management and how GitHub serves as a centralized platform for collaboration, backup, and automation.

### Learning Objectives

After completing this project, you will be able to:

- Understand the purpose of Git and GitHub
- Initialize a Git repository
- Configure your Git identity
- Track and stage file changes
- Create meaningful commits
- Create and manage GitHub repositories
- Connect local repositories to remote repositories
- Push code from a local machine to GitHub
- Understand the basic Git workflow

### Architecture

    Local Files
     │
     ▼
    Git Repository
     │
     ▼
    Commit History
     │
     ▼
    GitHub Repository

### Prerequisites

Before starting, ensure you have:

- Git installed
- GitHub account
- Terminal (Git Bash, PowerShell, macOS Terminal, or Linux Shell)
- Text Editor (Visual Studio Code recommended)

Verify Git installation:

    git --version    

### Step 1: Create a Project Directory

Create a new project folder:

    mkdir my-first-project
    cd my-first-project

Create a sample file:

    echo "<h1>Hello GitHub</h1>" > index.html

At this stage, the project exists only on your local machine.  

### Step 2: Initialize a Git Repository

Initialize Git:

    git init

This creates a hidden .git directory that stores all version control metadata.

Verify repository status:

    git status

### Step 3: Configure Git Identity

Configure your Git username:

    git config --global user.name "Your Name"

Configure your Git email address:

    git config --global user.email "you@example.com"

Verify your configuration:

    git config --list

Git uses this information to identify the author of every commit.  

### Step 4: Stage Files

Add files to Git's staging area:

    git add .

Check the repository status:

    git status

Expected output:

Changes to be committed:
    new file: index.html

### Step 5: Create Your First Commit

Create a commit:

    git commit -m "Initial commit"

View commit history:

    git log

A commit acts as a snapshot of your project at a specific point in time. 

### Step 6: Create a GitHub Repository

- Sign in to GitHub.
- Click New Repository.
- Enter a repository name.
- Choose Public or Private.
- Do not initialize with a README.
- Click Create Repository.

Example repository URL:

    https://github.com/lota001/local-to-github.git

### Step 7: Connect Local Repository to GitHub

Add the GitHub repository as a remote:

    git remote add origin https://github.com/lota001/local-to-github.git

Verify the connection:

    git remote -v


### Step 8: Push Code to GitHub

Rename the branch to main:

    git branch -M main

Push the repository:

    git push -u origin main

The -u flag establishes upstream tracking, allowing future pushes to be performed using:

    git push

Refresh GitHub and your project files should now be visible in the repository.

### NOTE

Making Future Changes

Modify your project files and repeat the Git workflow:

Check Status
         
     git status
Stage Changes

     git add .
Create Commit

    git commit -m "Added new feature"
Push Changes

    git push

### Conclusion

Git and GitHub are essential tools in modern software development and DevOps workflows. Understanding how to move code from a local machine to a GitHub repository establishes the foundation for more advanced practices such as Continuous Integration (CI), Continuous Delivery (CD), Infrastructure as Code (IaC), and collaborative software engineering.

Workflow Summary

    Create Files
     ↓
    git init
     ↓
    git add .
     ↓
    git commit
     ↓
    Create GitHub Repository
     ↓
    git remote add origin
     ↓
    git push -u origin main

Mastering this workflow is a critical first step toward becoming an effective developer, cloud engineer, or DevOps professional.
    
