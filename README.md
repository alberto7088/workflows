# workflows

This repository contains reusable GitHub Actions workflows, designed to streamline and automate common CI/CD tasks across projects.



Each file inside `.github/workflows/` defines a specific workflow for continuous integration, testing, building, or deployment.

## 🚀 Available Workflows

- **terraform_deployment.yml**
  Handles the deployment of your application to a specified environment.

*(More workflows can be added or customized as needed.)*

## 🛠️ Usage

You can reuse these workflows by referencing them from your other repositories.

Example usage:

```yaml
name: Reusable Build

on:
  push:
    branches:
      - main

jobs:
  build:
    uses: alberto7088/workflows/.github/workflows/build.yml@main
