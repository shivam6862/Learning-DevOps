# Configuring-Jenkins

## Creating your First Jenkins Job

### Steps:

1. **Job Configuration:**

   - Go to Jenkins dashboard and click "New Item."
   - Enter a name for the job and select the type of project (e.g., Freestyle project).

2. **Build Triggers:**
   - Under Build Triggers, select "Build periodically."
   - Add `H 23 * * *` inside the Schedule field to schedule the job at 11 PM every day.

## Adding a Build Step

### Overview:

A build step defines actions to be performed during the build process.

### Steps:

1. **Build Section:**
   - In the job configuration, go to the "Build" section.
   - Add build steps based on the requirements (e.g., shell commands, script execution).

## Adding Post-Build Actions

### Overview:

Post-build actions are tasks performed after the build is completed.

### Steps:

1. **Post-Build Actions Section:**
   - In the job configuration, go to the "Post-Build Actions" section.
   - Add actions such as archiving artifacts, sending notifications, or triggering other jobs.

## Configuring the Jenkins SMTP Server

### Overview:

Configuring the SMTP server enables Jenkins to send email notifications.

### Steps:

1. **Manage Jenkins:**

   - In the Jenkins dashboard, go to "Manage Jenkins" > "Configure System."

2. **Email Notification:**
   - Scroll down to the "E-mail Notification" section.
   - Enter the SMTP server details, including the server, user, and authentication.

## Running a Jenkins Job

### Steps:

1. **Build Now:**
   - In the Jenkins dashboard, select the desired job.
   - Click on "Build Now" to manually trigger the job.

## Jenkins Build Log

### Overview:

The Jenkins build log provides details about the execution of a job.

### Steps:

1. **Console Output:**
   - In the job details page, click on "Console Output" to view the build log.

## Jenkins Home Directory

### Overview:

The Jenkins home directory stores configuration, job information, and other essential data.

### Location:

The home directory is typically located at `/var/lib/jenkins` on Linux systems.

## Jenkins Backup and Restore

### Overview:

Backing up and restoring Jenkins ensures data recovery in case of system failure.

### Steps:

1. **Backup:**

   - Copy the Jenkins home directory to a safe location.

2. **Restore:**
   - Replace the current Jenkins home directory with the backup.

## Creating a Jenkins Job to Take Periodic Backup

### Steps:

1. **Job Configuration:**
   - Create a new Freestyle project.
   - Add a build step to execute a script that backs up the Jenkins home directory.

## Restoring a Jenkins Backup

### Steps:

1. **Stop Jenkins:**

   - Stop the Jenkins service.

2. **Replace Home Directory:**

   - Replace the current Jenkins home directory with the backup.

3. **Start Jenkins:**
   - Start the Jenkins service.

## Upgrading Jenkins

### Upgrading Jenkins Running on the Tomcat Server

### Steps:

1. **Download Latest Version:**

   - Download the latest Jenkins WAR file.

2. **Stop Jenkins:**

   - Stop the Tomcat server.

3. **Replace WAR File:**

   - Replace the existing Jenkins WAR file with the new one.

4. **Start Jenkins:**
   - Start the Tomcat server.

### Upgrading Standalone Jenkins Master on Windows

### Steps:

1. **Download Latest Version:**

   - Download the latest Jenkins installer for Windows.

2. **Run Installer:**
   - Run the installer and follow the upgrade wizard.

## Script to Upgrade Jenkins on Windows

### Script Example:

- Stop-Service -Name "Jenkins"
- $JenkinsInstaller = "https://updates.jenkins.io/download/war/latest/jenkins.war"
- Invoke-WebRequest -Uri $JenkinsInstaller -OutFile "C:\Program Files (x86)\Jenkins\jenkins.war"
- Start-Service -Name "Jenkins"

## Managing Jenkins Plugins

### Overview:

Jenkins plugins enhance functionality and integrations.

### Steps:

1. **Manage Jenkins:**

   - In the Jenkins dashboard, go to "Manage Jenkins" > "Manage Plugins."

2. **Install or Update Plugins:**
   - Use the "Available" or "Installed" tab to manage plugins.

## Installing a Jenkins Plugin to Take Periodic Backup

### Steps:

1. **Manage Jenkins:**

   - Go to "Manage Jenkins" > "Manage Plugins."

2. **Available Plugins:**

   - Navigate to the "Available" tab and search for a backup plugin.

3. **Install Plugin:**
   - Select the plugin and click "Install without restart."

## Enabling Global Security on Jenkins

### Overview:

Enabling global security enhances Jenkins' access control and authentication.

### Steps:

1. **Manage Jenkins:**

   - Go to "Manage Jenkins" > "Configure Global Security."

2. **Security Configuration:**
   - Configure security settings, including authentication and authorization.

## Using the Project-based Matrix Authorization Strategy

### Overview:

Matrix-based security allows fine-grained access control for Jenkins projects.

### Steps:

1. **Manage Jenkins:**

   - Go to "Manage Jenkins" > "Configure Global Security."

2. **Authorization:**
   - Select "Project-based Matrix Authorization Strategy" and configure user permissions.
