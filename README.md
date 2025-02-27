# shell-scripting
iam practicing shell scripting daily based
shell scripting with the same structured approach. We'll cover the basics, some practical examples, and how you can use shell scripting effectively in your role as an Azure DevOps Engineer.
Introduction to Shell Scripting
Shell scripting is a powerful tool to automate repetitive tasks, manage system operations, and streamline processes. Shell scripts are essentially text files containing a sequence of commands that the shell (like Bash) executes.
Basic Shell Scripting Concepts
Shebang (#!): Indicates the interpreter to be used (e.g., #!/bin/bash for Bash).
Variables: Store and manipulate data.
Control Structures: Use if, for, while to control the flow of the script.
Functions: Define reusable blocks of code.
Example 1: Simple Hello World Script
Let's start with a basic script that prints "Hello, World!" to the terminal.
Create and Edit the Script File:
sh
vim hello_world.sh


Script Content:
sh
#!/bin/bash
echo "Hello, World!"


Save and Exit:
Press Esc, type :wq, and press Enter.
Make the Script Executable:
sh
chmod +x hello_world.sh


Run the Script:
sh
./hello_world.sh


Example 2: Automating File Backup
Let's create a script to automate file backup similar to our Python example.
Create and Edit the Script File:
sh
vim backup_script.sh


Script Content:
sh
#!/bin/bash

# Define source and destination directories
SOURCE_DIR="/path/to/source_folder"
BACKUP_DIR="/path/to/backup_folder"

# Get the current date and time for the backup folder name
CURRENT_TIME=$(date +"%Y-%m-%d_%H-%M-%S")
BACKUP_PATH="$BACKUP_DIR/backup_$CURRENT_TIME"

# Create the backup folder
mkdir -p "$BACKUP_PATH"

# Copy files from source to backup folder
cp -r "$SOURCE_DIR/"* "$BACKUP_PATH/"

echo "Backup completed. Files are copied to $BACKUP_PATH"


Save and Exit:
Press Esc, type :wq, and press Enter.
Make the Script Executable:
sh
chmod +x backup_script.sh


Run the Script:
sh
./backup_script.sh


Using Shell Scripting in Azure DevOps
Automating Deployments: Shell scripts can automate the deployment process on Azure Kubernetes Service (AKS), setting up necessary resources like namespaces, deployments, and services.
Integrating with CI/CD: Use shell scripts in Azure Pipelines to automate build and deployment steps. Here's an example YAML pipeline definition that runs a shell script:
yaml
trigger:
- main

pool:
  vmImage: 'ubuntu-latest'

steps:
- script: |
    echo "Running shell script"
    ./backup_script.sh
  displayName: 'Run Backup Script'


System Monitoring: Write scripts to monitor system performance and generate alerts based on specific criteria.
Practice Exercises
Automate Log Rotation:
Write a script to archive and compress log files older than a week.
Schedule the script using cron to run daily.
Deploy Azure Resources:
Write a script to create Azure resources using az CLI commands.
Integrate the script into an Azure Pipeline.
