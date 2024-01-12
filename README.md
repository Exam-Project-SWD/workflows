# GitHub Actions workflows

This repository contains a collection of reusable GitHub Actions workflows for the organization.

They may require secrets or inputs to be passed from the calling workflow.
Since we are working within the same organization, we should be able to use `secrets: inherit` for convenience.

## Workflows

- [test.yml](.github/workflows/test.yml) - Setup Java and run Maven tests.
- [test_mysql.yml](.github/workflows/test_mysql.yml) - Setup Java and MySQL and run Maven tests.
- [deploy.yml](.github/workflows/deploy.yml) - Build Docker image and push to Docker Hub.
