# DevOps Git Project – Git Workflow Documentation

## 1. Project Overview
This project demonstrates a complete Git and GitHub workflow using branches, commits, pull requests, merge conflicts, conflict resolution, and Git history. The main objective is to understand how developers manage features safely using Git and GitHub.

## 2. Repository Structure
The repository contains the following important files:

- `.gitignore` – Specifies files that Git should ignore.
- `README.md` – Contains the project documentation.
- `feature.txt` – Contains the feature-related work.
- `git-workflow.md` – Contains Git workflow information.
- `branches.jpg` – Branch creation and management screenshot.
- `conflict-details.jpg` – Merge conflict details.
- `conflict-resolved.jpg` – Resolved merge conflict.
- `conflict.txt` – File used for demonstrating the conflict.
- `feature.txt` – Feature branch work.
- `final-git-history.jpg` – Final Git history.
- `github-repository.jpg` – GitHub repository screenshot.
- `merge-conflict.jpg` – Merge conflict demonstration.

## 3. Branching Strategy
The project follows a simple Git branching workflow:

`main → dev → feature/project-setup`

The `main` branch represents the final stable version.  
The `dev` branch is used for development and integration.  
The `feature/project-setup` branch is used to develop a specific feature without directly modifying the main branch.

## 4. Feature Development
A feature branch was created from the development branch and the required changes were added.

```bash
git checkout dev
git checkout -b feature/project-setup
git add .
git commit -m "Add project setup feature"
git push -u origin feature/project-setup

The feature branch was then pushed to GitHub and a Pull Request was created from:

feature/project-setup → dev

After reviewing the changes, the Pull Request was merged into the dev branch.

5. Merge Conflict Demonstration

A merge conflict was intentionally created to understand how Git handles changes made to the same file from different branches.

The conflict was inspected using:

git status
git diff

Git identified the conflicting section using conflict markers:

<<<<<<< HEAD
Current branch changes
=======
Incoming branch changes
>>>>>>> branch-name

The unwanted changes were removed and the correct content was kept.

6. Conflict Resolution

After resolving the conflict manually, the file was staged and committed.

git add .
git status
git commit -m "Resolve merge conflict"

The resolved changes were then pushed to GitHub.

The conflict-resolution screenshots are included in this repository as evidence.

7. Pull Request and Merge to Main

After completing development and resolving conflicts, the updated dev branch was merged into the main branch through a Pull Request.

Workflow:

feature/project-setup
        ↓
      dev
        ↓
      main

This workflow ensures that feature development is completed and tested before changes reach the stable main branch.

8. Git History Verification

The final repository history was verified using:

git log --oneline --all --graph --decorate

This command displays commits, branches, merges, and the overall project history in a graphical format.

The repository contains the completed Git workflow with feature development, merge operations, conflict resolution, and final integration.

9. Screenshots / Evidence

The following screenshots provide evidence of the completed workflow:

github-repository.jpg – GitHub repository
branches.jpg – Git branches
merge-conflict.jpg – Merge conflict
conflict-details.jpg – Conflict details
conflict-resolved.jpg – Conflict resolution
final-git-history.jpg – Final Git history
10. Conclusion

This project demonstrates practical knowledge of Git and GitHub including repository management, branching, feature development, commits, pushing changes, Pull Requests, merge conflicts, conflict resolution, and Git history verification.

The completed workflow follows:

Create Repository → Create Branches → Develop Feature → Commit → Push → Pull Request → Merge → Resolve Conflicts → Verify Git History → Final Main Branch

Author

Sindhupriya





