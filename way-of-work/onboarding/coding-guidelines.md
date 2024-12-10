# Voding Guidelines

## Repositories

1. Github --> url
2. Bitbucket --> url
3. GitLab --> url
4. Azure DevOps --> url

## Branching Strategy

Our branching strategy is designated by GitHub Flow. 

The most stable branch is the `main` branch (normally representing production). All new work should start by creating a `feature` branch that stems directly from main. The goal is to isolate the new feature, which is then merged into `main` by creating a Pull Request (PR).

The main goal behind this strategy is keeping the `main` code in a constant deployable state and hence can support continuous integration and continuous delivery processes.


1. Start a new feature by creating a new feature branch from the main branch.
2. Commit and push your code regularly.
3. When the new feature is ready to be merged into the main branch you must open a Pull Request; 
    - The code review should be done by a different person from the PR author;
    - Only open the PR when you think the code is ready to be reviewed (until then you can put your PR in draft);
    - Rule of thumb #1:  feature branches should have a short time to live (1 to 2 days) in order to avoid branches proliferation;
    - Rule of thumb #2: the PRs should be small as possible. We want easy and fast code reviews (aka small batchs);
4. The reviewer can ask for code changes or approve the PR;
5. The PR author is the one that is responsible for merging the PR after getting the approval;

## Banch naming convention

_**main branch**_

Most stable branch. Always ready to be deployed in production.

_**feature branch**_

Represents a new feature (a piece of work) that will be merged into `main`.

Feature branches should be created using the following convention: 

```
feature/JIRA-ID_name-of-the-feature
```

Examples:
- feature/JIRA-123
- feature/JIRA-123_login

_**hotfix branch**_

Represents a correction of a feature that needs to be merged into main.

Fix branches should be created using the following convention:

```
fix/JIRA-ID_name-of-the-feature
```

Examples:

fix/JIRA-123
fix/JIRA-123_login