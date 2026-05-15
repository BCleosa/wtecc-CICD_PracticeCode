# CI/CD Pipeline Final Project

## Project Name: CI/CD Pipeline with GitHub Actions, Tekton, and OpenShift

## Description
This project demonstrates a complete CI/CD pipeline implementation using:
- **GitHub Actions** for automated linting and unit testing
- **Tekton** for task management and pipeline orchestration
- **OpenShift** for application deployment

## Tech Stack
- **Runtime**: Node.js
- **Testing**: Jest
- **Linting**: ESLint
- **CI/CD**: GitHub Actions + Tekton
- **Platform**: OpenShift (IBM Skills Network)

## Pipeline Overview

### GitHub Actions Workflow
- **Lint Step**: ESLint to enforce code quality
- **Unit Test Step**: Jest to run automated tests

### Tekton Pipeline
- **Cleanup Task**: Remove previous deployments/resources
- **Test Task**: Run Jest unit tests inside the cluster

## Repository Structure
```
.
├── .github/
│   └── workflows/
│       └── workflow.yml       # GitHub Actions CI workflow
├── .tekton/
│   └── tasks.yml              # Tekton pipeline tasks
├── src/                       # Application source code
├── tests/                     # Jest test files
├── package.json
└── README.md
```

## How to Run Locally

### Install dependencies
```bash
npm install
```

### Run linting
```bash
npm run lint
```

### Run unit tests
```bash
npm test
```

## OpenShift Deployment
The application is deployed on OpenShift using Tekton pipelines.
Pipeline name: `oc-pipelines-oc-final`

## Author
CI/CD Final Project — IBM Developer Skills Network / Coursera
