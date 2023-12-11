# Setting-up-Jenkins

## What is Jenkins made of?

### Overview:

Jenkins is an open-source automation server widely used for building, deploying, and automating any project. It is made up of several key components:

1. **Core:**

   - The core of Jenkins provides the fundamental functionality, including building and triggering jobs.

2. **Plugins:**

   - Jenkins relies heavily on plugins, which extend its capabilities. Plugins cover integrations with version control systems, build tools, deployment platforms, and more.

3. **User Interface (UI):**

   - Jenkins has a web-based user interface for easy configuration and monitoring of jobs.

4. **Job Configuration:**
   - Jobs define tasks or processes to be executed. They include information such as source code repositories, build steps, and post-build actions.

## Jenkins Job

### Overview:

A Jenkins job is a defined task or a set of tasks that Jenkins executes. It can include activities such as pulling code from a version control system, compiling code, running tests, and deploying artifacts.

## Jenkins Parameters

### Overview:

Jenkins parameters are variables that can be defined for a job. They allow for customization and flexibility when running jobs. Parameters can be user input, environment variables, or predefined values.

## Jenkins Build

### Overview:

The Jenkins build process involves compiling source code, running tests, and generating artifacts. It is a fundamental step in the CI/CD pipeline and can be triggered manually or automatically upon code changes.

## Jenkins Post-Build Actions

### Overview:

Post-build actions in Jenkins are tasks performed after the build is completed. They can include steps like archiving artifacts, sending notifications, or triggering downstream jobs.

## Jenkins Pipeline

### Overview:

Jenkins Pipeline is a powerful feature that allows defining the entire build, test, and deployment process as code. It uses a domain-specific language (DSL) to describe the pipeline stages, providing flexibility and version control for the entire process.

## Why Use Jenkins as a Continuous Integration Server?

### Key Advantages:

- **Open Source:**

  - Jenkins is free and open source, making it accessible to a wide range of users.

- **Extensibility:**

  - Jenkins' extensive plugin ecosystem allows integration with a variety of tools and technologies.

- **Community Support:**

  - A large and active community contributes to plugins, support, and documentation.

- **Customization:**
  - Jenkins provides a high level of customization, allowing users to tailor their CI/CD processes.

## Jenkins as a Centralized Continuous Integration Server

### Overview:

Jenkins can act as a centralized CI server, managing and orchestrating the entire CI/CD pipeline. It provides a single point of control for building, testing, and deploying applications.

## Running Jenkins Inside a Container

### Overview:

Running Jenkins inside a container, using tools like Docker, allows for easy deployment and scalability. It provides isolation and portability across different environments.

## Installing Jenkins as a Service on the Apache Tomcat Server

### Overview:

Running Jenkins as a service on Apache Tomcat involves deploying Jenkins as a web application. It provides a scalable and efficient way to manage Jenkins in a production environment.

## Setting up Jenkins on Windows

### Steps:

1. **Download Jenkins:**

   - Download the Jenkins installer for Windows from the official website.

2. **Install Jenkins:**

   - Run the installer and follow the installation wizard.

3. **Configure Jenkins:**

   - Access Jenkins through a web browser, set up an admin account, and configure initial settings.

4. **Install Plugins:**

   - Choose and install relevant plugins to extend Jenkins functionality.

5. **Create a Job:**
   - Define a new job, configure source code repositories, build steps, and post-build actions.

## Setting up Jenkins on Ubuntu, Fedora

### Steps:

1. **Update Package Lists:**

   - Update the package lists on Ubuntu or Fedora.

2. **Install Java:**

   - Jenkins requires Java. Install OpenJDK or Oracle JDK.

3. **Add Jenkins Repository:**

   - Add the Jenkins repository to the package manager.

4. **Install Jenkins:**

   - Use the package manager to install Jenkins.

5. **Start Jenkins Service:**

   - Start the Jenkins service and enable auto-start on boot.

6. **Access Jenkins Web UI:**

   - Open a web browser, access Jenkins, and complete the initial setup.

7. **Install Plugins:**

   - Install necessary plugins for your use case.

8. **Create a Job:**
   - Define a new job, configure source code repositories, build steps, and post-build actions.
