
# Filtered Command History with Details, Notes, and Bash Prompts

### 1. **File Operations**

- **Listing files and directories:**
  - `ls`: Lists files in the current directory.
  - `ls -l`: Detailed list view, showing file permissions, size, and date.
  - `ls -a`: Shows hidden files as well (those starting with `.`).

- **Navigating directories:**
  - `cd /`: Changes to the root directory.
  - `cd /home/ubuntu/`: Changes to the `ubuntu` user directory.
  - `cd scripts/`: Moves into the `scripts` directory.

- **Creating directories:**
  - `mkdir scripts`: Creates a new directory named `scripts`.
  - `mkdir git-for-devops`: Creates a `git-for-devops` directory.

- **Creating files:**
  - `touch file1.txt file2.txt`: Creates two empty files, `file1.txt` and `file2.txt`.
  - `touch file3.txt`: Creates an empty file named `file3.txt`.
  - `touch uatfile.txt`: Creates an empty file named `uatfile.txt`.

- **Viewing file contents:**
  - `cat authorized_keys`: Displays the contents of the `authorized_keys` file.
  - `cat hello.txt`: Shows the content of the `hello.txt` file.

- **Removing files:**
  - `rm file1.txt`: Deletes `file1.txt` from the directory.

- **Editing files:**
  - `vim hello.sh`: Opens or creates the `hello.sh` script for editing using Vim.
  - `vim hello.txt`: Opens or creates the `hello.txt` file.
  - `vim file1.txt`: Edits `file1.txt` in Vim editor.

**Bash Prompt for Learning:**
```bash
# Navigate to the desired directory
cd /home/ubuntu/

# Create and list a new directory
mkdir my_project
ls

# Create a new script and edit it with vim
touch my_script.sh
vim my_script.sh
# Inside Vim, press 'i' to insert and write your bash script, e.g.:
# #!/bin/bash
# echo "Hello, world!"
# Save and exit: press 'ESC', then type ':wq' and press Enter

# View the contents of the script
cat my_script.sh
```

**Note:** Understanding how to manage files and directories is essential for automating tasks and scripting in Linux. The use of `vim` helps in directly editing files, while `ls`, `cat`, and `rm` help in managing file contents and structure.

---

### 2. **System Information and Disk Usage**

- **Disk space usage:**
  - `df -h`: Shows the disk space usage in a human-readable format.

- **Viewing system status:**
  - `systemctl status nginx.service`: Displays the status of the NGINX service, whether it's running, stopped, or failed.

**Bash Prompt for Learning:**
```bash
# Check available disk space
df -h

# View the status of a system service
sudo systemctl status nginx.service
```

**Note:** `df -h` helps you keep track of disk usage, especially when you're running out of space. `systemctl` is critical for managing services on Linux systems.

---

### 3. **Package Management (Ubuntu)**

- **Update and upgrade system:**
  - `sudo apt-get update`: Updates the list of available packages and their versions.
  - `sudo apt upgrade`: Installs newer versions of the packages you have.

- **Installing and removing software:**
  - `sudo apt-get install nginx`: Installs the NGINX web server.
  - `sudo apt purge nginx`: Removes the NGINX package from the system.

**Bash Prompt for Learning:**
```bash
# Update package list
sudo apt-get update

# Upgrade all installed packages
sudo apt upgrade

# Install a new package (e.g., nginx)
sudo apt-get install nginx

# Remove a package (e.g., nginx)
sudo apt purge nginx
```

**Note:** Regular updates are crucial for security patches and package improvements. Using `apt-get` allows you to manage software efficiently.

---

### 4. **System Administration**

- **Checking and managing services:**
  - `systemctl status nginx.service`: Checks the status of the NGINX service.
  - `sudo systemctl start nginx.service`: Starts the NGINX service.
  - `sudo systemctl stop nginx.service`: Stops the NGINX service.

- **Viewing command history:**
  - `history`: Shows the list of commands previously executed in the terminal.

**Bash Prompt for Learning:**
```bash
# Start and stop a service (e.g., nginx)
sudo systemctl start nginx.service
sudo systemctl stop nginx.service

# View the history of commands
history
```

**Note:** Understanding how to control system services is crucial for system administrators. Knowing how to start, stop, and check the status of services keeps your system in check.

---

### 5. **Networking Commands**

- **Incorrect usage:**
  - `sysctl staus nginx` (corrected as `sysctl status nginx`): This command attempts to view NGINX's status, though `systemctl` is usually preferred for managing services.

**Bash Prompt for Learning:**
```bash
# Correct way to check status of nginx using systemctl
systemctl status nginx
```

**Note:** System and network administrators often use `systemctl` for managing services, which includes monitoring networking services like NGINX.

---

### 6. **Bash Scripting**

- **Checking bash path:**
  - `which bash`: Displays the path to the bash binary.

- **Creating and running a bash script:**
  - `vim hello.sh`: Edits a bash script file.
  - `chmod 774 hello.sh`: Grants read, write, and execute permissions to the owner and others on `hello.sh`.
  - `./hello.sh`: Executes the `hello.sh` script.

**Bash Prompt for Learning:**
```bash
# Check where the bash interpreter is located
which bash

# Create and run a simple bash script
vim hello.sh
# Inside the script, you can write:
# #!/bin/bash
# echo "Hello, World!"
chmod 774 hello.sh
./hello.sh
```

**Note:** Writing and executing bash scripts allows for task automation, which is a fundamental skill for any Linux user.

---

### 7. **Git Commands**

- **Git repository setup:**
  - `git init`: Initializes an empty Git repository.
  - `git config --global user.name "crypn33r"`: Sets the Git username globally.
  - `git config --global user.email "ny7374@gmail.com"`: Sets the Git email globally.

- **Checking status and logs:**
  - `git status`: Shows the current state of the working directory and staging area.
  - `git log`: Shows commit history.
  - `git log --oneline`: Displays a simplified, single-line commit history.
  - `git log --oneline --source`: Adds source information to the log.

- **Adding and committing files:**
  - `git add file1.txt`: Stages `file1.txt` for the next commit.
  - `git commit -m "adding file1 and file2"`: Commits staged changes with a message.

- **Branching:**
  - `git checkout -b dev`: Creates and switches to a new branch named `dev`.
  - `git branch`: Lists all branches in the repository.

**Bash Prompt for Learning:**
```bash
# Initialize a new git repository
git init

# Set global config details
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"

# Add files to the staging area and commit
git add file1.txt
git commit -m "First commit"

# View the git log in a compact format
git log --oneline

# Create a new branch and switch to it
git checkout -b feature_branch
```

**Note:** Git is vital for version control, making it easier to track changes, collaborate, and manage branches. These commands are frequently used for everyday Git workflows.

---

### 8. **History and Help**

- **Viewing command history:**
  - `history`: Shows all previous terminal commands executed in the current session.

- **Viewing help for commands:**
  - `man git log`: Opens the manual page for `git log`, detailing usage and options.

**Bash Prompt for Learning:**
```bash
# View command history
history

# View help for a specific command (e.g., git log)
man git log
```

**Note:** The `history` command helps you track your previous commands, which can be useful for repeating or troubleshooting. The `man` command provides a reference for any command’s usage and options.

---

### Summary:
This enhanced guide covers essential Linux operations, system management, networking, Git, and bash scripting commands. Each section is accompanied by prompts for practicing, allowing you to better understand the command usage in real-world scenarios.
