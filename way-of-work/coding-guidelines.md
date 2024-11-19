# Coding Guidelines

## Where to create your code repository

## Branching Strategy

Start a new feature by creating a new feature branch from the main branch.

Commit and push your code regularly.

When the new feature is ready to be merged into the main branch you must open a Pull Request; 

The code review should be done by a different person from the PR author;

Only open the PR when you think the code is ready to be reviewed (until then you can put your PR in draft);

Rule of thumb #1:  feature branches should have a short time to live (1 to 2 days) in order to avoid branches proliferation;

Rule of thumb #2: the PRs should be small as possible. We want easy and fast code reviews (aka small batchs);

The reviewer can ask for code changes or approve the PR;

The PR author is the one that is responsible for merging the PR after getting the approval;

Br


## Branch naming convention
main branch

Most stable branch. Always ready to be deployed in production.

feature branch

Represents a new feature (a piece of work) that will be merged into main.

Feature branches should be created using the following convention: 

feature/JIRA-ID_name-of-the-feature

Examples:

feature/JIRA-123

feature/JIRA-123_login

hotfix

Represents a correction of a feature that needs to be merged into main.

 Fix branches should be created using the following convention:

fix/JIRA-ID_name-of-the-feature

Examples:

fix/JIRA-123

fix/JIRA-123_login