# task-8-hello-java-maven
# Hello Java Maven

This is a simple Java HelloWorld application used to demonstrate a basic CI/CD pipeline using Jenkins and Maven.

## 📂 Project Structure

hello-java-maven/
├── pom.xml
└── src/
└── main/
└── java/
└── HelloWorld.java

markdown
Copy
Edit

## 🔧 Tools Used

- Java JDK 8
- Maven 3.8.6
- Jenkins (via Docker)
- Git & GitHub

## 🛠️ Jenkins Build Instructions

1. **Install Jenkins via Docker:**
   ```bash
   docker run -d -p 8080:8080 -p 50000:50000 --name jenkins -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts
Install Maven in Jenkins:

Go to Manage Jenkins → Global Tool Configuration.

Add Maven (e.g., Maven 3.8.6).

Create Freestyle Job:

Source Code Management: Git → Add your GitHub repo URL.

Build Step: Invoke top-level Maven targets

Goals: clean package

Build the job manually

✅ Output
If everything is set up correctly, Jenkins will compile your project, and the console output will end with [INFO] BUILD SUCCESS


