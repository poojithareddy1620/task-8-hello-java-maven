**Hello Java Maven**
**Overview**
A simple Java HelloWorld application built using Maven. This project demonstrates basic Java compilation and packaging and is integrated with Jenkins for automated CI/CD.

**Usage**
**Clone the repository**
git clone https://github.com/poojithareddy1620/task-8-hello-java-maven.git
cd task-8-hello-java-maven
**Build the project using Maven**
mvn clean package
**Run the compiled program**
java -cp target/hello-1.0.jar HelloWorld
**Expected Output**
Hello, Jenkins + Maven!
**Jenkins Integration**
This project is used in a Jenkins Freestyle job configured to:

Pull code from this GitHub repository

Run mvn clean package as the build step

Validate build success via Jenkins console output
