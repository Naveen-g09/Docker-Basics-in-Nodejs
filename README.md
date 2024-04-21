---

# Docker Basics in Node.js

This repository serves as a practical demonstration of various DevOps concepts, focusing on Docker, Node.js, TypeScript, and Continuous Integration/Continuous Deployment (CI/CD) pipelines using GitHub Actions.

## Overview

In this project, we cover the following topics:

1. **Docker**: Docker is utilized to containerize our Node.js application, ensuring consistency and portability across different environments. We create a Docker image to encapsulate our application and its dependencies.

2. **Node.js with TypeScript**: Our application is built using Node.js, a popular JavaScript runtime, along with TypeScript, which adds static typing to the language, enhancing code quality and developer productivity.

3. **Database Integration**: Our Node.js application interacts with a database, demonstrating how Docker can be used to manage complex development environments with multiple interconnected components.

4. **Volumes**: Docker volumes are employed to persist data, ensuring that database changes are retained even when containers are destroyed and recreated.

5. **GitHub Actions for CI/CD**: We implement Continuous Integration (CI) and Continuous Deployment (CD) pipelines using GitHub Actions. With every commit, a new Docker image is built and pushed to GitHub's container registry, facilitating automated testing and deployment workflows.

## Getting Started

To run the project locally, follow these steps:

1. **Clone the Repository**: 
    ```bash
    git clone https://github.com/Naveen-g09/Docker-Basics-in-Nodejs.git
    ```

2. **Navigate to Source Directory**: 
    ```bash
    cd Docker-Basics-in-Nodejs/src
    ```

3. **Install Dependencies**: 
    ```bash
    npm install
    ```

4. **Start the Server**: 
    ```bash
    npm run pm2
    npm run start
    ```

This will launch the Node.js server locally.

## Creating a Docker Image

To create a Docker image from the project, follow these steps:

1. **Navigate to the Root Directory** of the project.

2. **Build the Docker Image**:
    ```bash
    docker build -t <image_name> .
    ```

3. **Commit Changes and Push to GitHub**: 
    After building the Docker image locally, commit your changes and push them to GitHub. This will trigger the CI/CD pipeline configured with GitHub Actions, automatically building and pushing the Docker image to the GitHub container registry.

## Contributing

Contributions are welcome! If you have any suggestions, enhancements, or bug fixes, please feel free to open an issue or create a pull request.

---

Feel free to customize this README further to add any additional details or instructions you think are necessary.
