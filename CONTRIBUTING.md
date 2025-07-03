# Contributing to Space Robotics Lab Projects

Thank you for your interest in contributing to our work! These guidelines are designed to ensure that our collaborative process is smooth, consistent, and effective. Following them helps us maintain high-quality code and makes it easier for everyone to contribute.

## Table of Contents
1. [Code of Conduct](#code-of-conduct)
2. [Repository Naming Convention](#repository-naming-convention)
3. [Our Development Workflow](#our-development-workflow)
    - [Branching Strategy](#branching-strategy)
    - [Making Commits](#making-commits)
    - [Submitting a Pull Request](#submitting-a-pull-request)
4. [Coding Standards](#coding-standards)
5. [Issue Tracking](#issue-tracking)

## Code of Conduct
All members of this organization are expected to adhere to our [Code of Conduct](link-to-your-CODE_OF_CONDUCT.md-file). Please ensure you have read and understood it.

## Repository Naming Convention
To ensure our organization remains easy to navigate, all new repositories **must** follow a strict naming convention:

`[team-acronym]-[project-name]`

Please use lowercase letters, numbers, and hyphens only.

**Official Team Acronyms:**
* `oc-` (Orbital-Casting Team)
* `moon-` (Moon Team)
* `rover-` (Rover Team)
* `climb-` (CLIMB Team)

**Example:** A new project for the Rover team to test wheel designs should be named `rover-wheel-test-rig`.

## Our Development Workflow
We use a simple, branch-based workflow to manage contributions. The `main` branch is always kept in a stable, deployable state. All new work happens on separate feature branches.

### Branching Strategy
1.  **Never work directly on `main`**.
2.  Create a new branch for every new feature, bug fix, or experiment.
3.  Follow this naming convention for your branches:
    `[team-acronym]/feature/[short-description-of-work]`
    - **Good:** `oc/feature/add-debris-capture-simulation`
    - **Good:** `rover/feature/fix-pathfinding-bug`
    - **Bad:** `my-branch`, `fix`

    You can create a new branch locally with:
    ```bash
    git checkout -b oc/feature/my-new-feature
    ```

### Making Commits
- **Commit frequently:** Make small, logical commits. This makes your changes easier to review.
- **Write clear commit messages:** We follow a conventional commit style. Your message should have a type, a scope (the project), and a clear subject.
    - `feat(oc-pipeline): Add new kalman filter for state estimation`
    - `fix(rover-nav): Correct odometry calculation error`
    - `docs(haptics-firmware): Update README with setup instructions`

### Submitting a Pull Request (PR)
When your feature or fix is complete:
1.  **Push your branch** to the repository on GitHub.
2.  **Open a Pull Request** against the `main` branch.
3.  **Fill out the PR template:** Your PR description should clearly explain *what* you changed and *why*. Link to any relevant issues (e.g., "Closes #42").
4.  **Request a review:** Assign at least one other member from your team or the `maintainers` team as a reviewer.
5.  **Address feedback:** The reviewer may request changes. Make the required changes on your branch and push them. The PR will update automatically.
6.  **Merge:** Once the PR is approved, a maintainer will merge it into the `main` branch. Delete your feature branch after the merge is complete.

## Coding Standards
To maintain consistency across our projects, we adhere to the following standards:
- **Python:** All Python code must follow the [PEP 8 Style Guide](https://www.python.org/dev/peps/pep-0008/). We recommend using a linter like `flake8` to check your code.
- **Documentation:** All functions should have clear docstrings explaining their purpose, arguments, and return values.
- *(Add any other lab-specific standards here, e.g., for C++, MATLAB, etc.)*

## Issue Tracking
- **Bugs:** If you find a bug, please create an issue in the relevant repository. Use the "Bug Report" template and provide as much detail as possible, including steps to reproduce it.
- **Feature Requests:** For new ideas, create an issue using the "Feature Request" template. Explain the problem you want to solve and your proposed solution.

---
Thank you for helping us build better research software!
