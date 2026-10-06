# DevOps Git Project

## 📌 Project Overview

This project demonstrates the practical usage of **Git and GitHub** for version control and collaborative software development.

The project covers important Git concepts such as:

- Repository creation
- Git configuration
- Branching
- Feature development
- Pull Requests
- Merge conflicts
- Conflict resolution
- Git workflow
- Tags and releases
- `.gitignore`
- Commit history
- Collaboration using GitHub

The complete workflow was implemented using a GitHub repository and documented with screenshots.

---

## 👩‍💻 Author

**Sindhupriya Abbineni**

GitHub: [@sindhupriya5e1](https://github.com/sindhupriya5e1)

---

# 🛠️ Technologies Used

- Git
- GitHub
- Git Bash
- GitHub Pull Requests
- Markdown
- Visual Studio Code

---

# 📂 Repository Structure

The repository contains the following important files:

```text
devops-git-project/
│
├── .gitignore
├── README.md
├── branches.jpg
├── conflict-details.jpg
├── conflict-resolved.jpg
├── conflict.txt
├── feature.txt
├── final-git-history.jpg
├── git-workflow.md
├── github-repository.jpg
├── merge-conflict.jpg
├── new-change.txt
├── new-change-2.txt
├── pr-change.txt
├── pull-request-conflict-resolution.jpg
├── pull-request-dev-to-main.jpg
└── pull-request-feature-to-dev.jpg
1. GitHub Repository Creation
A GitHub repository named devops-git-project was created to perform and document the Git activities.

The repository was created as a public repository.

Repository Screenshot

2. Git Initialization and Project Setup
The project was initialized as a Git repository and connected with GitHub.

The basic Git workflow followed in this project was:

Working Directory
       ↓
     Git Add
       ↓
   Staging Area
       ↓
   Git Commit
       ↓
 Local Repository
       ↓
   Git Push
       ↓
     GitHub
Git was used to track all changes made to the project.

3. Git Branching
Branches were created to keep different development activities separate.

The repository contains multiple branches, including:

main

dev

feature

The main branch represents the stable version of the project.

The dev branch was used for development and integration.

The feature branch was used to implement individual feature changes.

Branch Screenshot

4. Feature Branch Development
A separate feature branch was created for making feature-related changes.

The feature branch allowed changes to be developed independently without directly modifying the main branch.

Example file used:

feature.txt
The feature changes were committed to the feature branch.

5. Pull Request: Feature → Dev
After completing the feature development, a Pull Request was created to merge the feature branch into the development branch.

Pull Request Flow
feature
   ↓
Pull Request
   ↓
dev
Screenshot

This process demonstrates how developers can review and integrate feature changes before adding them to the development branch.

6. Pull Request Changes
Additional changes were created and committed during the development process.

Files such as:

new-change.txt
new-change-2.txt
pr-change.txt
were used to demonstrate Pull Request changes.

These changes were committed and pushed to the appropriate branch.

7. Pull Request: Dev → Main
After the development work was completed and verified, a Pull Request was created to merge the development branch into the main branch.

Pull Request Flow
dev
 ↓
Pull Request
 ↓
main
Screenshot

This represents the final integration of the development work into the stable main branch.

8. Merge Conflict
A merge conflict occurs when Git cannot automatically combine changes from different branches.

In this project, a merge conflict was intentionally created to demonstrate how conflicts can be identified and resolved.

The conflict was created in:

conflict.txt
Merge Conflict Screenshot

9. Conflict Details
When the conflicting branches were merged, Git identified conflicting changes.

The conflict contained Git conflict markers similar to:

<<<<<<< HEAD
Current branch changes
=======
Incoming branch changes
>>>>>>> branch-name
The conflicting content was reviewed manually before deciding which changes should be retained.

Conflict Details Screenshot

10. Conflict Resolution
The conflicting content was manually corrected by removing the unwanted changes and Git conflict markers.

After resolving the conflict, the corrected file was staged and committed.

The general conflict resolution process was:

Identify Conflict
       ↓
Open Conflicting File
       ↓
Review Changes
       ↓
Resolve Conflict
       ↓
git add
       ↓
git commit
       ↓
Push Changes
Resolved Conflict Screenshot

11. Pull Request Conflict Resolution
A Pull Request conflict was also handled as part of the project.

The conflict was resolved before completing the merge.

Screenshot

This demonstrates the practical process of handling conflicts during collaborative GitHub development.

12. Git Workflow
The complete Git workflow followed in this project is:

Create Repository
       ↓
Clone Repository
       ↓
Create Branch
       ↓
Make Changes
       ↓
Git Add
       ↓
Git Commit
       ↓
Git Push
       ↓
Create Pull Request
       ↓
Review Changes
       ↓
Resolve Conflicts if Required
       ↓
Merge Pull Request
       ↓
Update Main Branch
A detailed explanation of the workflow is available in:

git-workflow.md
Git Workflow Documentation

13. Git Commit History
Git commits were used to maintain a history of changes made throughout the project.

Each commit represents a logical change in the project.

The repository contains multiple commits demonstrating:

Initial project setup

Branch creation

Feature changes

Pull Request changes

Conflict creation

Conflict resolution

Documentation updates

Screenshot uploads

Final Git History

14. .gitignore
A .gitignore file was added to the repository.

The purpose of .gitignore is to prevent unnecessary or unwanted files from being tracked by Git.

For example:

node_modules/
.env
*.log
dist/
build/
The .gitignore file helps keep the repository clean and prevents sensitive or generated files from being accidentally committed.

15. GitHub Repository Files
The final repository contains the documentation files, text files, screenshots, and Git configuration files required for demonstrating the complete workflow.

Important files include:

File	Purpose
.gitignore	Specifies files ignored by Git
README.md	Project documentation
feature.txt	Feature branch changes
conflict.txt	File used for conflict demonstration
new-change.txt	Pull Request change
new-change-2.txt	Additional Pull Request change
pr-change.txt	Pull Request demonstration
git-workflow.md	Git workflow documentation
16. Screenshots
GitHub Repository

Branches

Feature to Dev Pull Request

Dev to Main Pull Request

Merge Conflict

Conflict Details

Conflict Resolved

Pull Request Conflict Resolution

Final Git History

17. Learning Outcomes
Through this project, the following concepts were practically demonstrated:

Understanding Git fundamentals

Creating and managing Git repositories

Creating and switching branches

Working with feature branches

Making and tracking changes

Creating meaningful commits

Pushing changes to GitHub

Creating Pull Requests

Merging branches

Understanding merge conflicts

Resolving conflicts manually

Reviewing Git history

Using .gitignore

Documenting projects using Markdown

Following a collaborative Git workflow

18. Complete Git Workflow Summary
The overall workflow implemented in this project can be summarized as:

                 GitHub Repository
                        │
                        ▼
                      main
                        │
                        ▼
                       dev
                        │
             ┌──────────┴──────────┐
             │                     │
             ▼                     │
          feature                  │
             │                     │
             ▼                     │
        Feature Changes            │
             │                     │
             ▼                     │
       Pull Request                │
             │                     │
             └──────────► dev ◄────┘
                           │
                           ▼
                    Conflict Handling
                           │
                           ▼
                    Conflict Resolution
                           │
                           ▼
                    Pull Request
                           │
                           ▼
                         main
19. Conclusion
This project demonstrates a complete practical Git and GitHub workflow starting from repository creation and branching to Pull Requests, merge conflicts, conflict resolution, and final integration.

The project provides hands-on experience with Git version control and demonstrates how GitHub can be used for collaborative software development.

The documented workflow can be applied to real-world development projects where multiple developers work on different branches and integrate their changes through Pull Requests.

✅ Project Completed
Repository: devops-git-project

Owner: sindhupriya5e1

Branching: main, dev, feature

Key Concepts Covered:

✅ Git Repository
✅ GitHub
✅ Branching
✅ Feature Development
✅ Commits
✅ Pull Requests
✅ Merge Conflicts
✅ Conflict Resolution
✅ Git Workflow
✅ Git History
✅ .gitignore
✅ Project Documentation

🔗 GitHub Repository
View the DevOps Git Project


