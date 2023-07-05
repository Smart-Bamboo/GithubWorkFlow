# How We Work
This document outlines the guidelines and best practices for collaborating on this GitHub organization. It covers the processes, tools, and conventions that we follow to ensure effective teamwork and efficient development.

## Table of Contents
- [Communication](#communication)
- [Issue Tracking](#issue-tracking)
- [Branching Strategy](#branching-strategy)
- [Conventional Commits](#conventional-commits)
- [Code Review](#code-review)
- [Documentation](#documentation)
- [Continuous Integration](#continuous-integration)
- [Deployment](#deployment)


## Communication

We primarily use [Slack](https://slack.com/) for day-to-day communication and collaboration. Please join our team workspace and join relevant channels to stay updated and engaged with the team.

## Issue Tracking

We use the GitHub issue tracker to manage and track our work. If you encounter a bug, have an idea for an improvement, or need to request a new feature, please open an issue in this repository.

## Branching Strategy

We follow the [Gitflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) branching model for our development workflow. The main branches in this repository are:

- `main`: The main branch represents the production-ready codebase. It should always contain stable code.
- `dev`: The develop branch is where new features and bug fixes are tested before being merged into the main branch.
- Feature branches: For each new feature or bug fix, create a new branch from the `main` branch. Use descriptive branch names and prefix them with a feature or bug number.

## Conventional Commits

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification for our commit messages. This convention helps provide a consistent structure to our commit messages and enables automated processes such as generating changelogs and versioning.

When making commits to this repository, please adhere to the following guidelines:

- Use imperative verbs in the commit message. For example, "Fix bug" instead of "Fixed bug" or "Fixes bug."
- Separate the subject from the body with a blank line.
- Use the subject line to provide a concise summary of the changes.
- Include the Jira or issue number in the subject line if applicable. For example, "[JIRA-123] Add new feature" or "[#42] Fix bug."
- Add a detailed description in the body if necessary. Include any relevant information, such as the motivation for the change, additional context, or breaking changes.

Following this convention helps maintain a clear commit history and improves collaboration among team members.

To automate our release process and generate changelogs automatically, we use tools such as [Conventional Commits CLI](https://www.npmjs.com/package/conventional-commits-cli) or [Commitizen](https://commitizen.github.io/cz-cli/). These tools provide interactive prompts to guide you through creating conventional commits.

Remember that well-formed commit messages contribute to better code understanding, easier debugging, and streamlined release processes.

## Code Review

Code reviews are an essential part of our development process. Before merging any code into `main` branche, it must be reviewed by at least one team member. Follow these steps for code review:

1. Create a pull request (PR) from your feature branch to the `main` branch.
2. Assign the PR to a team member for review.
3. The reviewer will provide feedback, suggest improvements, and discuss any necessary changes.
4. Once the code is approved, the reviewer will merge the PR into the target branch.

## Documentation

We value clear and concise documentation to maintain a well-documented codebase. Document important concepts, architectural decisions, APIs, and any other relevant information to facilitate understanding and maintainability. We use Markdown for documentation.

## Continuous Integration

We have set up a continuous integration (CI) pipeline to automatically build, test, and analyze our code. The CI process is triggered whenever a pull request is opened or updated. Ensure that all tests pass, and any required checks or quality standards are met before merging your code.

## Deployment

We have a defined deployment process to ensure a smooth release of our code. The process includes the following steps:

1. Once the code is merged into the `main` branch, it undergoes final testing and quality checks.
2. The deployment is triggered automatically by our CI/CD pipeline, which packages and deploys the code to the production environment.
3. We closely monitor the deployment process and perform any necessary post-deployment verification.
4. In case of any issues or unexpected behavior after deployment, we have a rollback strategy in place to revert to a stable state if needed.

By following this deployment process, we ensure that our code is safely released to our users and any potential disruptions are minimized.


Happy collaborating!
