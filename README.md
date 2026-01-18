# Nexus Artifact Demo

This project demonstrates how to set up **Nexus Repository Manager**, create users and repositories, and publish Java artifacts using **Gradle** and **Maven**.  

It is designed for learning backend and DevOps concepts without installing heavy tools locally.

---

## Tech Stack

- Java 17
- Gradle
- Maven
- Nexus Repository Manager
- Docker
- GitHub Codespaces (free cloud environment)
- Linux

---

## Project Overview

### 1. Nexus Setup
- Ran Nexus in a Docker container on Codespaces
- Logged in with admin account
- Disabled anonymous access
- Created two hosted repositories:
  - `java-gradle-releases`
  - `java-maven-releases`
- Created a developer user with proper permissions

### 2. Gradle Project
- Created a Java application with Gradle
- Built a JAR using `gradle build`
- Configured publishing to Nexus
- Uploaded artifact using `gradle publish`

### 3. Maven Project
- Generated a Java Maven project
- Built JAR using `mvn package`
- Configured `pom.xml` to publish to Nexus
- Uploaded artifact using `mvn deploy`

---

## How to Run

### Gradle Project
```bash
cd gradle-project
gradle build
gradle publish
```

### Maven Project
```bash
cd maven-app
mvn package
mvn deploy
```
