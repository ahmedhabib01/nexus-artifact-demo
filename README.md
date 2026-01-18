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





Maven Project
cd maven-app
mvn package
mvn deploy


Artifacts will appear in Nexus under the respective repositories.

What You Will Learn

How Nexus works and why it is used

How to create repositories and users

Publishing artifacts using Gradle and Maven

Free cloud development workflow (Codespaces + Docker)

Basics of DevOps and backend pipeline setup

Future Improvements

Add CI/CD workflow for automatic builds and uploads

Add finer permissions for Nexus users

Add a multi-module Gradle project

Add a frontend and backend integration demo

License

MIT
