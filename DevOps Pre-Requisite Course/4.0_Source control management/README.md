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
