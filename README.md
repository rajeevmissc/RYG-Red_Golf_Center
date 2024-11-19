# RYG-Red_Golf_Center
# Development Process Guide

## Table of Contents
- [Getting Started](#getting-started)
- [Development Environment Setup](#development-environment-setup)
- [Git Workflow](#git-workflow)
- [Pull Request Process](#pull-request-process)
- [Conflict Resolution](#conflict-resolution)

## Getting Started

### Prerequisites
- Git installed on your local machine
- GitHub account with access to the repository
- Required development tools (listed in Development Environment Setup)

### Initial Setup
1. Clone the repository:
```bash
git clone https://github.com/organization/project-name.git
cd project-name
```

2. Set up your Git identity:
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

## Development Environment Setup

1. Install required dependencies:
   - Node.js (v16.x or later)
   - npm or yarn
   - Docker (for containerized development)

2. Install project dependencies:
```bash
npm install
# or
yarn install
```

3. Set up environment variables:
```bash
cp .env.example .env
# Edit .env with your local configuration
```

## Git Workflow

### Branch Naming Convention
- Feature branches: `feature/description-of-feature`
- Bug fixes: `fix/description-of-bug`
- Hotfixes: `hotfix/description-of-hotfix`

### Daily Development Flow

1. Update your local main branch:
```bash
git checkout main
git pull origin main
```

2. Create a new feature branch:
```bash
git checkout -b feature/your-feature-name
```

3. Make your changes and commit regularly:
```bash
git add .
git commit -m "feat: description of your changes"
```

4. Push your branch to remote:
```bash
git push -u origin feature/your-feature-name
```

### Commit Message Format
Follow Conventional Commits specification:
```
type(scope): description

[optional body]

[optional footer]
```

Types:
- feat: New feature
- fix: Bug fix
- docs: Documentation changes
- style: Code style changes
- refactor: Code refactoring
- test: Adding tests
- chore: Maintenance tasks

### Branching Strategy
- `main`: Production-ready code
- Feature branches: Individual development work
- Hotfix branches: Production fixes

## Pull Request Process

1. Create Pull Request (PR):
   - Go to GitHub repository
   - Click "New Pull Request"
   - Select your feature branch as source
   - Select `main` as target
   - Fill out the PR template

2. PR Requirements:
   - Clear title and description
   - Link to related issues
   - Passing CI/CD checks
   - Updated documentation
   - Test coverage
   - No merge conflicts

3. Review Process:
   - Request reviews from team members
   - Address feedback
   - Update PR as needed
   - Get required approvals

4. Merging:
   - Squash and merge preferred
   - Delete branch after merging

## Conflict Resolution

### Preventing Conflicts
- Pull from main regularly
- Keep branches short-lived
- Communicate with team about file changes

### Resolving Conflicts

1. Update your branch:
```bash
git checkout feature/your-feature
git fetch origin
git rebase origin/main
```

2. If conflicts occur:
```bash
# Fix conflicts in your editor
git add .
git rebase --continue
```

3. Force push if necessary:
```bash
git push --force-with-lease origin feature/your-feature
```

## Additional Resources
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)
- [Conventional Commits](https://www.conventionalcommits.org/)

## Need Help?
- Contact: `rajeevm@issc.co.in`
- Slack: #development-help




## Installation

To install dependencies use npm

```bash
  npm install
```
Backend / Server start command: 
```bash
  npm run start
  Nodemon index
```

Frontend / Client start command: 
```bash
  npm run dev
```








