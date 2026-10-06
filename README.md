# DevOps Git Version Control Project

---

## Project Overview

This project demonstrates Git and GitHub best practices for managing a DevOps project using version control. It covers repository management, branching, feature development, pull requests, merging, conflict resolution, tagging, and project documentation.

## Objectives

- Understand Git fundamentals
- Create and manage branches
- Follow a feature-based Git workflow
- Use Pull Requests
- Merge branches
- Resolve merge conflicts
- Use `.gitignore`
- Create Git tags
- Use Git stash
- Document tasks using Markdown

## Tools Used

- Git
- GitHub
- Git Bash
- Visual studio code
- Markdown

## Branching Strategy

| Branch | Purpose |
|--------|---------|
| `main` | Stable production-ready code |
| `dev` | Development and integration |
| `feature/*` | Individual feature development |

## Git Workflow

```text
feature → dev → main
The project follows a feature-based Git workflow. Individual features are developed in feature branches and integrated into the development branch. After testing and verification, the changes are merged into the main branch.

Project Structure
devops-git-task4/
│── README.md
│── .gitignore
│
└── screenshots/
    ├── 01-github-repository.jpg
    ├── 02-branches.jpg
    ├── 03-feature-branch.jpg
    ├── 04-commits.jpg
    ├── 05-pull-request-feature.jpg
    ├── 06-pull-request-dev.jpg
    ├── 07-merge-conflict.jpg
    ├── 08-conflict-details.jpg
    ├── 09-conflict-resolved.jpg
    ├── 11-pull-request-confirmed.jpg
    └── 12-final-git-history.jpg
Tasks
Git repository initialization

Branch creation

Feature development

Git commits

GitHub repository management

Pull Requests

Branch merging

Merge conflict resolution

Git tags

Git stash

.gitignore

Markdown documentation

Key Git Concepts Demonstrated
Git repository initialization and remote configuration

Feature-based branching strategy

Main, development, and feature branches

Git commits and version history

Pull Request workflow

Branch merging

Merge conflict identification and resolution

.gitignore for excluding unnecessary files

Git stash for temporarily storing changes

Annotated Git tags and versioning

Markdown-based project documentation

Git Commands Used
git init
git clone
git status
git add .
git commit
git branch
git checkout
git switch
git merge
git pull
git push
git log
git stash
git tag
git remote -v
Version
v1.0.0 – Final version of the DevOps Git Version Control Project.

Outcome
This project demonstrates practical Git and GitHub version-control workflows used in DevOps environments. It provides hands-on experience with branching, commits, pull requests, merging, conflict resolution, tagging, and documentation.

Author
Sindhupriya

BTech | Cloud & DevOps Enthusiast
