# Hello Java Maven Project

This is a simple Java HelloWorld application built with Maven, used to demonstrate a Jenkins CI/CD pipeline.

## Project Structure

- `src/main/java/HelloWorld.java`: Java source code that prints a message.
- `pom.xml`: Maven configuration file that manages project build and dependencies.

## Prerequisites

- Java JDK 8 or 11
- Maven
- Jenkins (with Maven plugin configured)

## How to Build Locally

1. Clone the repository:

```bash
git clone https://github.com/poojithareddy1620/task-8-hello-java-maven.git
cd task-8-hello-java-maven
**Build the project using Maven:**
mvn clean package
**Run the compiled program:**
java -cp target/hello-1.0.jar HelloWorld
**You should see the output:**
Hello, Jenkins + Maven!

Jenkins Integration
This project is used in a Jenkins freestyle job configured to:

Pull code from this GitHub repo

Run mvn clean package as the build step

Validate the build status in Jenkins console
