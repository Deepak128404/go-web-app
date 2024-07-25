# Go Web Application

This is a simple website written in Golang. It uses the `net/http` package to serve HTTP requests.

## Running the server

To run the server, execute the following command:

```bash
go run main.go
```

The server will start on port 8080. You can access it by navigating to `http://localhost:8080/courses` in your web browser.

## Looks like this

![Website](static/images/golang-website.png)

# Go Web App CI/CD Pipeline 🚀

This repository contains a simple Go web application with a comprehensive CI/CD pipeline implemented using GitHub Actions, Helm, and ArgoCD.

## CI/CD Overview 🌟

### Continuous Integration (CI) 🔄

The CI pipeline is implemented using GitHub Actions and includes the following steps:

1. **Code Build and Test**: Automatically builds and tests the Go application. 🛠️
2. **Static Code Analysis**: Runs static code analysis tools to ensure code quality. 🔍
3. **Docker Image Build**: Builds a Docker image for the application. 🐳
4. **Docker Image Push**: Pushes the Docker image to Docker Hub. 📦

### Continuous Deployment (CD) 🚚

The CD pipeline is implemented using Helm and ArgoCD, following a GitOps approach:

1. **Helm Chart**: Defines the Kubernetes manifests for deploying the application. 📜
2. **ArgoCD**: Automatically syncs the Helm chart with the Kubernetes cluster. 🔄

## Getting Started 🛠️

### Prerequisites

- Docker installed and running 🐳
- Kubernetes cluster set up ☸️
- ArgoCD installed in the Kubernetes cluster 🔄
- Docker Hub account 📦

### Workflow

1. **CI Pipeline**:
   - Push code changes to the repository. 📝
   - GitHub Actions will automatically trigger the CI pipeline. 🔄
   - The pipeline will build and test the code, run static code analysis, build the Docker image, and push it to Docker Hub. 📦

2. **CD Pipeline**:
   - Update the Helm chart with any necessary changes. 📜
   - Push the Helm chart updates to the repository. 📝
   - ArgoCD will automatically sync the changes to the Kubernetes cluster. 🔄

## GitHub Actions Workflow 🛠️

The GitHub Actions workflow is defined in `.github/workflows/ci.yml`. It includes the following jobs:

- **build**: Builds and tests the Go application. 🛠️
- **lint**: Runs static code analysis. 🔍
- **docker**: Builds and pushes the Docker image to Docker Hub. 🐳

## Helm Chart 📜

The Helm chart is located in the `helm` directory. It includes the necessary Kubernetes manifests for deploying the application.

## ArgoCD 🔄

ArgoCD is configured to sync the Helm chart with the Kubernetes cluster.

## Contributing 🤝

Feel free to contribute to this project by opening issues or submitting pull requests.

## License 📜

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.




