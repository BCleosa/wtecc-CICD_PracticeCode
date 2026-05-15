(
echo # CI/CD Pipeline Final Project
echo.
echo **Project Name:** CI/CD Pipeline with GitHub Actions, Tekton, and OpenShift
echo.
echo ## Description
echo.
echo This project demonstrates a complete CI/CD pipeline implementation using:
echo.
echo - **GitHub Actions** for automated linting and unit testing
echo - **Tekton** for task management and pipeline orchestration
echo - **OpenShift** for application deployment
echo.
echo ## Tech Stack
echo.
echo ^| Component ^| Tool ^|
echo ^|--------^|--------^|
echo ^| Runtime ^| Node.js ^|
echo ^| Testing ^| Jest ^|
echo ^| Linting ^| ESLint ^|
echo ^| CI/CD ^| GitHub Actions + Tekton ^|
echo ^| Platform ^| OpenShift (IBM Skills Network) ^|
echo.
echo ## Pipeline Overview
echo.
echo ### GitHub Actions Workflow
echo.
echo - **Lint Step:** ESLint to enforce code quality
echo - **Unit Test Step:** Jest to run automated tests
echo.
echo ### Tekton Pipeline
echo.
echo - **Cleanup Task:** Remove previous deployments and resources
echo - **Git Clone Task:** Clone the repository
echo - **Lint Task:** Run ESLint inside the cluster
echo - **Test Task:** Run Jest unit tests inside the cluster
echo - **Build Task:** Build container image using Buildah
echo - **Deploy Task:** Deploy application to OpenShift
echo.
echo ## Repository Structure
echo.
echo ```
echo .
echo ├── .github/
echo │   └── workflows/
echo │       └── workflow.yml
echo ├── .tekton/
echo │   └── tasks.yml
echo ├── src/
echo ├── tests/
echo ├── package.json
echo └── README.md
echo ```
echo.
echo ## How to Run Locally
echo.
echo ### Install dependencies
echo.
echo ```bash
echo npm install
echo ```
echo.
echo ### Run linting
echo.
echo ```bash
echo npm run lint
echo ```
echo.
echo ### Run unit tests
echo.
echo ```bash
echo npm test
echo ```
echo.
echo ## OpenShift Deployment
echo.
echo - **Pipeline name:** oc-pipelines-oc-final
echo - **Persistent Volume Claim:** Storage class skills-network-learner, capacity 1Gi
echo - **Application port:** 8000
echo.
echo ## Author
echo.
echo CI/CD Final Project — IBM Developer Skills Network / Coursera
) > README.md
