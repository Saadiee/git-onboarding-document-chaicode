# Welcome to Git and GitHub at ChaiCode Cohort!  

Congratulations on joining the ChaiCode Cohort team! This guide is designed to help you get started with Git and GitHub, two essential tools for efficient and collaborative software development. Whether you're new to these tools or need a refresher, this guide will walk you through installation, setup, and best practices to ensure you're ready to contribute to our projects.

## Why Git and GitHub?

### **Git**  
Git is a powerful version control system that tracks changes in your codebase. It enables multiple developers to collaborate on a project, manage versions, and maintain a detailed history of modifications. With Git, you can experiment with new features without affecting the main codebase, and rollback changes if something goes wrong.

### **GitHub**  
GitHub is a web-based platform built around Git. It serves as a centralized space for storing, sharing, and managing code repositories. It’s indispensable for team collaboration, offering tools like pull requests, issue tracking, and code reviews.

By mastering Git and GitHub, you'll work more effectively with your team and contribute seamlessly to ChaiCode's innovative projects.

---

## Getting Started with Git and GitHub

### Installation and Setup

#### **Step 1: Install Git**
Follow these steps to install Git on your operating system:

**For Windows**  
1. Download the Git installer from [git-scm.com](https://git-scm.com/).  
2. Run the installer and follow the prompts.  
   - On the “Adjusting your PATH environment” screen, choose “Git from the command line and also from 3rd-party software.”  
   - Keep the default settings for other options unless specified by your system admin.  
3. Complete the installation and verify by running:
   ```bash
   git --version
   ```

**For macOS**  
1. Install Git using Homebrew:
   ```bash
   brew install git
   ```
2. Verify the installation:
   ```bash
   git --version
   ```

**For Linux**  
1. Use your package manager to install Git:
   ```bash
   sudo apt update
   sudo apt install git
   ```
2. Verify the installation:
   ```bash
   git --version
   ```

#### **Step 2: Configure Git**
Set your username and email to identify your contributions:
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

#### **Step 3: Create a GitHub Account**
1. Visit [github.com](https://github.com/) and click **Sign Up**.  
2. Complete the registration process and verify your email.  
3. Once your account is set up, share your GitHub username with your team lead to be added to the ChaiCode organization.

---

## Cloning the ChaiCode Repository

To begin working on ChaiCode projects, you’ll need to clone the repository.  

1. Copy the repository URL from GitHub (e.g., `https://github.com/ChaiCode/example-repo.git`).  
2. Open a terminal and run:
   ```bash
   git clone https://github.com/ChaiCode/example-repo.git
   ```
3. Navigate into the cloned repository:
   ```bash
   cd example-repo
   ```

---

## Basic Git Commands

Here are some common Git commands you’ll use regularly:

### **Check Repository Status**
```bash
git status
```

### **Stage Changes**
```bash
git add <file>  # Stage a specific file
git add .       # Stage all changes
```

### **Commit Changes**
```bash
git commit -m "Your descriptive message"
```

### **Push Changes to Remote Repository**
```bash
git push
```

### **Pull Latest Changes**
```bash
git pull
```

### **View Commit History**
```bash
git log
```

---

## Writing Commit Messages

Follow these guidelines for meaningful commit messages:
- **Use present tense:** "Add feature" not "Added feature."
- **Capitalize** the first word.
- Keep messages concise (50 characters or less).  
- Use prefixes for categorization:  
  - `feat:` for features  
  - `fix:` for bug fixes  
  - `docs:` for documentation changes  
  - Example:  
    ```bash
    feat: Add tea selection feature  
    fix: Resolve login issue for tea enthusiasts  
    docs: Update README with chai varieties  
    ```

---

## Branching Workflow at ChaiCode

We use the following branching strategy:  
1. **`main` branch**: Always deployable. Contains stable code.  
2. **`development` branch**: Contains the latest changes under review.  
3. **Feature branches**: Used for new features, named as `feature/<feature-name>`.  

### **Create and Switch Branches**
```bash
git branch feature/tea-menu
git checkout feature/tea-menu
```

### **Merge Branches**
1. Switch to the target branch (e.g., `development`):
   ```bash
   git checkout development
   ```
2. Merge the feature branch:
   ```bash
   git merge feature/tea-menu
   ```
3. Push the changes:
   ```bash
   git push
   ```

### **Resolve Conflicts**  
If conflicts occur, Git will notify you. Open the conflicting files, resolve issues, and mark them as resolved:
```bash
git add <file>
git commit
```

---

## Creating Pull Requests (PR)

1. Push your branch to GitHub:
   ```bash
   git push origin feature/tea-menu
   ```
2. Navigate to the repository on GitHub.  
3. Click **New Pull Request** and select your branch.  
4. Add a title and description summarizing the changes.  
5. Request reviews from your team.  

---

## Best Practices

- **Commit Often**: Regular commits make it easier to track changes and debug issues.  
- **Write Descriptive Messages**: Help teammates understand your changes at a glance.  
- **Pull Regularly**: Always pull the latest changes before starting new work to avoid conflicts.  
