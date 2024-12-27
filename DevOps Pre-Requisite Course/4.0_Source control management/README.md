# Source Control Management (SCM) with Git

This document provides an introduction to Git, a popular SCM tool, and essential commands for DevOps professionals.

---
## What is Git?

Git is a distributed version control system that allows you to track changes in code over time. It offers several advantages over traditional SCM systems, including:

- **Version Control**: Git keeps a history of all changes made to your code, enabling you to revert to previous versions if necessary.
- **Distributed Workflow**: Each developer has a complete copy of the repository, facilitating offline work and collaboration.
- **Branching**: Git allows you to create branches for independent development, making it easier to experiment with new features without affecting the main codebase.
- **Merging**: Once you're satisfied with changes in a branch, you can merge them back into the main codebase.

---
## Getting Started with Git

Here’s a basic workflow for using Git:

1. **Initialize a Repository**:  
   Use `git init` to create a new Git repository in your project directory.

2. **Track Changes**:  
   Use `git add <file>` to stage files for your next commit. This tells Git which files you want to include in the version history.

3. **Commit Changes**:  
   Use `git commit -m "descriptive message"` to create a snapshot of the staged changes with a descriptive message.

4. **Remote repository (optional)**:
   Push your local commits to a remote repository like GitHub or GitLab for collaboration and version control across teams:
   ```bash
   git remote add origin <remote_repository_url>
   git push origin <branch_name>
   ```

   ## Collaboration

- **Clone a remote repository**:
  ```bash
  git clone <remote_repository_url>
  ```
  Creates a local copy of the remote repository.

- **Pull updates from the remote repository**:
  ```bash
  git pull origin <branch_name>
  ```
  Gets the latest changes from other collaborators.

- **Create branches for your work**:
  ```bash
  git checkout -b <branch_name>
  ```
  Switches to a new branch for independent development.

- **Merge branches**:
  ```bash
  git merge <branch_name>
  ```
  Merges changes from another branch.

  ## Helpful Git Commands for DevOps

### Basic commands:
- `git init`: Initializes a new Git repository.
- `git status`: Shows the status of your working directory and staging area.
- `git add <file>`: Adds a file to the staging area.
- `git commit -m "message"`: Creates a commit with a message.
- `git log`: Shows the commit history.

### Branching commands:
- `git branch`: Lists all branches.
- `git checkout <branch_name>`: Switches to a different branch.
- `git branch -b <branch_name>`: Creates a new branch.
- `git merge <branch_name>`: Merges changes from another branch.

### Remote repository commands:
- `git remote add <name> <url>`: Adds a remote repository.
- `git push <remote_name> <branch_name>`: Pushes your local commits to a remote branch.
- `git pull <remote_name> <branch_name>`: Pulls changes from a remote branch.

## Additional Resources

- [Git SCM official documentation](https://git-scm.com/)
- [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials)
- [GitHub Guide](https://github.com/git-guides)

This document provides a foundational understanding of Git. As you delve deeper into DevOps practices, explore more advanced Git features and functionalities to streamline your development workflow.

