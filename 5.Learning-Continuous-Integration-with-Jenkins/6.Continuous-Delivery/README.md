# Continuous Delivery Using Jenkins

## What is Continuous Delivery?

### Overview:

Continuous Delivery (CD) is a software engineering approach that aims to automate and streamline the process of delivering software to production in a reliable and efficient manner. It goes beyond Continuous Integration by extending automation to the entire software delivery lifecycle, including testing, deployment, and release.

## Continuous Delivery Design

### Overview:

The design of Continuous Delivery involves creating a streamlined and automated workflow for software delivery. It encompasses the architecture, tools, and processes required to achieve a reliable and repeatable delivery pipeline.

## Continuous Delivery Pipeline

### Overview:

The Continuous Delivery pipeline is a series of automated steps and processes that software goes through from development to production. It includes stages such as building, testing, deploying, and releasing software, ensuring a consistent and efficient delivery process.

### Pipeline to Poll the Feature Branch

#### Steps:

1. **Pipeline Script:**

   - Write a Jenkins pipeline script to poll the feature branch for changes.

2. **Build and Test:**
   - Include stages in the pipeline for building and testing the code.

### Pipeline to Poll the Integration Branch

#### Steps:

1. **Pipeline Script:**

   - Write a Jenkins pipeline script to poll the integration branch for changes.

2. **Merge and Test:**
   - Include stages for merging changes from feature branches into the integration branch and testing.

## Toolset for Continuous Delivery

### Components:

1. **Java:**
   - Programming language.
2. **Apache JMeter:**

   - Tool for performance testing.

3. **Apache Tomcat Server:**

   - Servlet container for deploying applications.

4. **Jenkins:**

   - CI/CD automation server.

5. **Artifactory:**

   - Artifact repository.

6. **SonarQube:**
   - Code quality and static analysis tool.

### Configuring Our Testing Server

#### Steps:

1. **Installing Java on the Testing Server:**

   - Install Java on the server.

2. **Installing Apache JMeter for Performance Testing:**

   - Download and install JMeter.

3. **Creating a Performance Test Case:**

   - Define a performance test case using JMeter.

4. **Installing Apache Tomcat Server on the Testing Server:**
   - Set up Tomcat on the server.

## Jenkins Configuration

### Steps:

1. **Configuring the Performance Plugin:**

   - Set up Jenkins to report and visualize performance test results.

2. **Configuring the TestNG Plugin:**

   - Configure Jenkins to integrate with TestNG for testing.

3. **Changing Jenkins/Artifactory/Sonar Web URLs:**

   - Modify web URLs for Jenkins, Artifactory, and Sonar in Jenkins configuration.

4. **Modifying the Maven Configuration:**

   - Adjust Maven settings in Jenkins.

5. **Modifying the Java Configuration:**

   - Configure Java settings in Jenkins.

6. **Modifying the Git Configuration:**

   - Set up Git configurations in Jenkins.

7. **Configuring Jenkins Slaves on the Testing Server:**
   - Configure Jenkins to use slaves on the testing server.

## Creating Jenkins Continuous Delivery Pipeline

### Steps:

1. **Modifying the Existing Jenkins Job:**

   - Enhance an existing Jenkins job to fit into the CD pipeline.

2. **Modifying the Advanced Project:**

   - Adjust configurations for more advanced CD requirements.

3. **Modifying the Jenkins Job for Integration Test and Static Code Analysis:**

   - Enhance the job for integration testing and static code analysis.

4. **Modifying the Jenkins Job for Uploading Packages to Artifactory:**
   - Adjust the job for uploading artifacts to Artifactory.

## Creating Jenkins Jobs for Specific Stages 55, 359, 367)

### Steps:

1. **Creating a Jenkins Job to Deploy Code on the Testing Server:**

   - Configure a job for deploying code on the testing server.

2. **Creating a Jenkins Job to Run UAT:**

   - Set up a job for running User Acceptance Testing (UAT).

3. **Creating a Jenkins Job to Run Performance Test:**
   - Configure a job for running performance tests.

## Creating a Nice Visual Flow for the Continuous Delivery Pipeline 71)

### Overview:

Visualizing the CD pipeline helps in understanding and monitoring the progress of code through different stages.

### Steps:

1. **Creating Visual Flow:**
   - Use tools or plugins to create a visual representation of the CD pipeline.

## Creating a Simple User Acceptance Test Using Selenium and TestNG 78)

### Steps:

1. **Installing TestNG for Eclipse:**

   - Install TestNG plugin for Eclipse.

2. **Modifying the index.jsp File:**

   - Make changes to the index.jsp file for testing purposes.

3. **Modifying the POM File:**

   - Adjust the Maven POM file to include necessary dependencies.

4. **Creating a User Acceptance Test Case:**

   - Develop a TestNG test case using Selenium for User Acceptance Testing.

5. **Generating the testng.xml File:**
   - Generate the TestNG XML configuration file.

## Continuous Delivery in Action

### Steps:

1. **Committing and Pushing Changes on the Feature1 Branch:**

   - Make code changes and commit them to the feature1 branch.

2. \*\*Jenkins Continuous

Delivery Pipeline in Action:\*\*

- Observe how the CD pipeline is triggered and progresses after code changes.

3. **Exploring Jobs for Deployment, UAT, and Performance Testing:**
   - Navigate through Jenkins to explore specific jobs related to deployment, UAT, and performance testing.
