
# Linux Commands Overview

---

## 1. File Operations
```bash
# Listing files and directories
ls
ls -l
ls -a

# Changing directory
cd /
cd /home/ubuntu/
cd scripts/

# Creating a directory
mkdir scripts
mkdir git-for-devops

# Creating a file
touch file1.txt file2.txt
touch file3.txt
touch uatfile.txt

# Viewing file contents
cat authorized_keys
cat hello.txt

# Deleting a file
rm file1.txt

# Editing files with vim
vim hello.sh
vim hello.txt
vim file1.txt
```

---

## 2. System Information and Disk Usage
```bash
# Display disk usage
df -h

# Display uptime
uptime

# Check memory usage
free -m

# System information
hostnamectl
whoami
```

---

## 3. Package Management (Ubuntu)
```bash
# Update package list
sudo apt-get update

# Upgrade installed packages
sudo apt upgrade

# Install a package (nginx)
sudo apt-get install nginx

# Remove a package (nginx)
sudo apt purge nginx
```

---

## 4. System Administration
```bash
# Checking status of nginx service
systemctl status nginx.service
systemctl status nginx

# Starting and stopping nginx service
sudo systemctl start nginx.service
sudo systemctl stop nginx.service

# Checking the status of a service
systemctl status nginx
```

---

## 5. Networking Commands
```bash
# Check system routing table
route

# Check IP address information
ip addr

# Bring up and down network interface
ip link set eth0 up
ip link set eth0 down

# Ping a host
ping google.com

# Display active connections
netstat

# DNS lookup
nslookup google.com

# Traceroute to a host
traceroute google.com
```

---

## 6. Bash Scripting
```bash
# Check bash location
which bash

# Writing and executing a bash script
vim hello.sh
chmod 774 hello.sh
./hello.sh
```

---

## 7. Git Commands
```bash
# Initialize a git repository
git init

# Check git status
git status

# Add files to git
git add file1.txt
git add file2.txt
git add hello.txt
git add uatfile.txt

# Remove file from git (cached)
git rm --cached file1.txt

# Commit changes
git commit -m "adding file1 and file2"
git commit -m "adding uatfile to uat branch"
git commit -m "adding file1,Hello.txt and file2"

# Git configuration
git config --global user.name "crypn33r"
git config --global user.email "ny7374@gmail.com"

# Check git log
git log
git log --oneline
git log --oneline --source

# Git branch operations
git checkout -b dev
git checkout master
git checkout dev
git branch
git checkout -b uat

# Git show and status
git show
git status
```

---

## 8. History and Help
```bash
# View command history
history

# Display manual for a command
man git log
```

---

# Conclusion

This list covers a range of basic Linux commands for file operations, system administration, networking, package management, Git usage, and more. Each command serves a specific purpose and is essential for working efficiently with Linux.

---
