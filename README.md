# Task 4 – Git & GitHub Workflow

## 1. Project Overview

This project demonstrates a complete Git and GitHub workflow using branches, commits, pull requests, merges, tags, `.gitignore`, and Markdown documentation.

The objective of this task is to understand how developers manage code changes using Git branches and collaborate through GitHub Pull Requests.

### Repository

**GitHub Repository:**
`https://github.com/sindhupriya5e1/devops-git-project`

---

## 2. Objectives

The main objectives of this task are:

* Create and configure a GitHub repository.
* Initialize a local Git repository.
* Create and manage different Git branches.
* Work on a feature branch.
* Push changes to GitHub.
* Create a Pull Request from the feature branch to `dev`.
* Merge the feature branch into `dev`.
* Create a Pull Request from `dev` to `main`.
* Merge the changes into `main`.
* Use `.gitignore` to exclude unnecessary files.
* Create Git tags for project versions.
* Document the complete Git workflow using Markdown.
* Maintain a clean and understandable repository structure.

---

# 3. Repository Setup

A new GitHub repository was created specifically for this task.

### Repository Name

`devops-git-project`

The repository was kept public so that the completed work and documentation could be reviewed.

The repository contains the project files, Git workflow documentation, README file, and `.gitignore`.

---

# 4. Project Structure

The final project structure is:

```text
devops-git-project/
│
├── README.md
├── .gitignore
├── index.html
    └──git workflow.md
```

### Description of Files

| File / Folder      | Purpose                                  |
| ------------------ | ---------------------------------------- |
| `README.md`        | Main project documentation               |
| `.gitignore`       | Files and folders that Git should ignore |
| `index.html`       | Basic project HTML file                  |
| `app.txt`          | Project/application information          |
| `src/`             | Source/project files                     |
| `docs/workflow.md` | Detailed Git workflow documentation      |

---

# 5. Git Initialization

The project was first initialized as a local Git repository.

```bash
git init
```

Git was then configured with the user's identity:

```bash
git config user.name "Your Name"
git config user.email "Your Email"
```

The repository status was checked using:

```bash
git status
```

This command helps identify new, modified, staged, and committed files.

---

# 6. Creating the Initial Project

The initial project files were created and added to Git.

Files included:

* `README.md`
* `.gitignore`
* `index.html`
* `app.txt`
* `src/`

The files were added to the staging area:

```bash
git add .
```

The first commit was then created:

```bash
git commit -m "Initial project setup"
```

This commit represents the initial version of the project.

---

# 7. Creating the Main Branch

The primary branch of the project is `main`.

The branch can be created or renamed using:

```bash
git branch -M main
```

The current branch can be checked using:

```bash
git branch
```

The `main` branch represents the stable version of the project.

---

# 8. Creating the Development Branch

A separate development branch was created to keep ongoing development changes away from the stable `main` branch.

```bash
git checkout -b dev
```

The branch structure is therefore:

```text
main
 │
 └── dev
```

The `dev` branch is used for development and testing before changes are moved to `main`.

---

# 9. Creating the Feature Branch

A separate feature branch was created from the development branch.

```bash
git checkout dev
git checkout -b feature/project-setup
```

The feature branch is:

```text
feature/project-setup
```

This branch was used to make the required project/documentation changes without directly modifying the `dev` or `main` branches.

---

# 10. Making Changes on the Feature Branch

The required project files and documentation were added or updated on the feature branch.

After making the changes, the repository status was checked:

```bash
git status
```

The changes were then staged:

```bash
git add .
```

A commit was created:

```bash
git commit -m "Add project setup documentation"
```

This created a separate commit for the project documentation and setup work.

---

# 11. Pushing the Feature Branch to GitHub

The feature branch was pushed to the GitHub repository:

```bash
git push -u origin feature/project-setup
```

After pushing, the feature branch became available on GitHub.

---

# 12. Creating Pull Request – Feature to Dev

A Pull Request was created on GitHub from:

```text
feature/project-setup
```

to:

```text
dev
```

The Pull Request allowed the changes to be reviewed before merging them into the development branch.

The workflow was:

```text
feature/project-setup
          │
          │ Pull Request
          ▼
         dev
```

After reviewing the changes, the Pull Request was merged.

---

# 13. Updating the Local Dev Branch

After the Pull Request was merged, the local `dev` branch was updated.

```bash
git checkout dev
git pull origin dev
```

This ensured that the local development branch contained the changes merged through GitHub.

---

# 14. Dev to Main Pull Request

Once the changes were available and verified in `dev`, another Pull Request was created.

The second Pull Request was:

```text
dev → main
```

This Pull Request represents the process of promoting tested development changes into the stable production branch.

The workflow was:

```text
feature/project-setup
          │
          │ PR
          ▼
         dev
          │
          │ PR
          ▼
         main
```

After review, the `dev` branch changes were merged into `main`.

---

# 15. Final Branch Structure

After completing the workflow, the important branches were:

```text
main
dev
```

The feature branch:

```text
feature/project-setup
```

was used for the feature work and was deleted after the Pull Request was successfully merged.

This keeps the repository clean after completing the feature.

---

# 16. .gitignore

A `.gitignore` file was included in the repository.

The purpose of `.gitignore` is to prevent unnecessary files from being tracked by Git.

Examples of files that can normally be ignored include:

```text
node_modules/
.env
*.log
.vscode/
.idea/
.DS_Store
```

The `.gitignore` file helps maintain a clean repository and prevents temporary or sensitive files from being committed accidentally.

---

# 17. Git Tags

Git tags are used to identify important versions of a project.

A tag can be created using:

```bash
git tag v1.0
```

The tags can be viewed using:

```bash
git tag
```

A tag can be pushed to GitHub using:

```bash
git push origin v1.0
```

The tag represents a stable version of the project.

---

# 18. Checking Git Status

Throughout the workflow, Git status was used to verify the repository state.

```bash
git status
```

This command helps confirm:

* Current branch
* Modified files
* Staged files
* Untracked files
* Clean working tree

A clean working tree indicates that all required changes have been committed.

---

# 19. Checking Branches

The branches can be viewed using:

```bash
git branch
```

Remote branches can be viewed using:

```bash
git branch -r
```

All local and remote branches can be viewed using:

```bash
git branch -a
```

This was useful for verifying the final branch structure.

---

# 20. Git Log

The project commit history can be viewed using:

```bash
git log --oneline --graph --all
```

This provides a visual representation of the commits and branches.

The project history contains commits such as:

```text
Initial project setup
Add project setup documentation
```

This demonstrates that the project changes were tracked through Git commits.

---

# 21. Complete Git Workflow

The complete workflow followed in this task can be represented as:

```text
                    main
                     ▲
                     │
                  PR / Merge
                     │
                     dev
                     ▲
                     │
                  PR / Merge
                     │
          feature/project-setup
                     │
                  Changes
                     │
                  Commit
                     │
                Local Git
```

The overall development process was:

```text
Create Repository
       ↓
Initialize Git
       ↓
Create main
       ↓
Create dev
       ↓
Create feature branch
       ↓
Make project changes
       ↓
git add
       ↓
git commit
       ↓
Push feature branch
       ↓
Feature → dev Pull Request
       ↓
Merge into dev
       ↓
Pull latest dev changes
       ↓
dev → main Pull Request
       ↓
Merge into main
       ↓
Create Git Tag
       ↓
Verify final repository
```

---

# 22. Verification

Before completing the task, the repository was checked to ensure:

* `main` branch exists.
* `dev` branch exists.
* Feature branch changes were merged.
* Feature branch was deleted after successful merge.
* Project files are available in the repository.
* `.gitignore` is present.
* `README.md` is present.
* `docs/workflow.md` is present.
* Git commits are visible.
* Pull Requests were completed.
* Final code is available on `main`.
* Git tag/version information is available.

---

# 23. Screenshots / Evidence

The following screenshots can be included as evidence for the completed task:

### Screenshot 1 – Repository

GitHub repository showing:

```text
devops-git-project
```

### Screenshot 2 – Git Initialization / Status

Terminal showing:

```bash
git init
git status
```

### Screenshot 3 – Branches

Terminal showing:

```bash
git branch
```

with `main`, `dev`, and the feature branch during development.

### Screenshot 4 – Feature Branch

GitHub/terminal showing:

```text
feature/project-setup
```

### Screenshot 5 – Commit History

Terminal showing:

```bash
git log --oneline --graph --all
```

### Screenshot 6 – Feature → Dev Pull Request

GitHub Pull Request showing:

```text
feature/project-setup → dev
```

and the successful merge.

### Screenshot 7 – Dev → Main Pull Request

GitHub Pull Request showing:

```text
dev → main
```

and the successful merge.

### Screenshot 8 – Final Branches

GitHub branches page showing the final:

```text
main
dev
```

branches.

### Screenshot 9 – Repository Files

GitHub repository showing:

```text
README.md
.gitignore
docs/
index.html
src/
app.txt
```

### Screenshot 10 – Git Tag

GitHub/terminal showing the created version tag.

---

# 24. Final Repository

The final GitHub repository is:

**Repository:** `devops-git-project`

**GitHub:**
https://github.com/sindhupriya5e1/devops-git-project

The repository demonstrates the complete Git workflow required for Task 4, including branching, commits, Pull Requests, merging, `.gitignore`, tags, and documentation.

---

# 25. Conclusion

Task 4 demonstrates a complete Git and GitHub based development workflow.

The project was developed using a feature branch, integrated into the `dev` branch through a Pull Request, and finally promoted to the `main` branch through another Pull Request.

The use of Git branches, commits, Pull Requests, `.gitignore`, tags, and Markdown documentation provides a structured and professional approach to source-code management.

The final repository contains the required project files and documentation and can be reviewed through the GitHub repository link provided above.
