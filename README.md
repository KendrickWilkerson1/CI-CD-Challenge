# 19 CI-CD: GitHub Actions CI/CD Setup

## Task

As applications scale and develop, developers want to ensure that certain quality checks are met prior to merging to important branches; thus, you'll want to familiarize yourself with Continuous Integration (CI) and Continuous Deployment (CD) that are common practices used to ensure consistency, quality, and deployment of latest code once all checks have been met and merged to `main`.

Your task is to create a CI/CD pipeline using GitHub Actions to run the component tests via Cypress when a Pull Request is made to the `develop` branch, and the application is deployed when code is merged from `develop` to the `main` branch.

## User Story

```md
AS A developer looking to integrate a pipeline in a codebase for continuous integration and deployment, 
I WANT to create a GitHub Action that will follow best practices by running test cases when a Pull Request is made to the develop branch
SO THAT I can ensure that all code integrations are clean and pass the proper requirements.

AS A developer looking to deploy the application automatically to Render when code is merged from develop to main,
I WANT to create a GitHub Action that will run when the code is merged to main and automatically deploys to Render
SO THAT the application is constantly updated when major releases are made to the main branch.
```

## Acceptance Criteria

```md
GIVEN a fullstack application for a web developer,
WHEN I upload new features to the application
THEN I should be making Pull Requests to a develop branch first
WHEN I create a Pull Request to a develop branch
THEN I should be executing a GitHub Action that checks the Cypress component tests
WHEN I see that the tests pass on GitHub Action
THEN I should see those test results on GitHub Action and merge the code
WHEN I push the code from the develop branch to the main branch
THEN I should see that another GitHub Action triggers and should automatically deploy to Render
```
