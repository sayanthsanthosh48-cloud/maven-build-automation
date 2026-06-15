# Build Automation and CI Pipeline with Maven & GitHub Actions

## Project Overview

This project demonstrates Build Automation and Continuous Integration (CI) using Apache Maven and GitHub Actions. A Java application was developed, built, tested, and packaged into a deployable JAR file using Maven. The entire build process is automated through a GitHub Actions workflow that runs whenever code is pushed to the repository.

The project was developed as part of a Cloud & DevOps learning journey to understand software build automation, dependency management, version control, and CI/CD fundamentals.

---

## Project Architecture

```text
Developer
    │
    ▼
GitHub Repository
    │
    ▼
GitHub Actions CI Pipeline
    │
    ▼
Maven Build Process
    │
    ├── Compile Source Code
    ├── Run Unit Tests
    ├── Package Application
    │
    ▼
JAR Artifact
```

---

## Technologies Used

* Java 17
* Apache Maven
* Git
* GitHub
* GitHub Actions
* AWS EC2 (Ubuntu Linux)

---

## Features

* Maven-based build automation
* Dependency management
* Automated compilation
* Unit testing
* JAR packaging
* Version control using Git
* Continuous Integration using GitHub Actions
* Automatic build execution on every push to the main branch

---

## Project Structure

```text
build-automation
│
├── .github
│   └── workflows
│       └── maven.yml
│
├── src
│   ├── main
│   │   └── java
│   └── test
│
├── pom.xml
├── .gitignore
└── README.md
```

---

## Maven Commands

### Compile the Project

```bash
mvn compile
```

### Run Unit Tests

```bash
mvn test
```

### Package the Application

```bash
mvn package
```

### Clean Build Files

```bash
mvn clean
```

---

## Running the Application

After packaging:

```bash
java -cp target/build-automation-1.0-SNAPSHOT.jar com.skillified.App
```

Expected Output:

```text
Build Automation Using Maven
Skillified Cloud & DevOps Internship Project
```

---

## GitHub Actions CI Pipeline

The project includes an automated GitHub Actions workflow located at:

```text
.github/workflows/maven.yml
```

The workflow automatically:

* Triggers on every push to the main branch
* Sets up Java 17
* Builds the project using Maven
* Runs tests
* Generates the deployable JAR artifact

---

## Learning Outcomes

Through this project, I gained hands-on experience with:

* Linux command-line operations
* Java application development
* Maven build lifecycle
* Dependency management
* Source code management using Git
* GitHub repository management
* Continuous Integration using GitHub Actions
* AWS EC2 environment setup and configuration

---

## Future Enhancements

* Integrate Jenkins CI/CD pipeline
* Dockerize the application
* Deploy containers on AWS EC2
* Implement Kubernetes orchestration
* Automate infrastructure provisioning using Terraform

---

## Author

Sayanth Santhosh

Cloud & DevOps Enthusiast
