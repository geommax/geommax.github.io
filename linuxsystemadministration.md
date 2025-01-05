# Linux Course Outline

## Course Overview

### This course is divided into three main sections:

1. **Linux System Administration**
2. **Linux Server Administration**
3. **Linux Security**

---

## Section 1: Linux System Administration

### Topics Covered:

- **Command Line Basics**
  - What is the command line in Linux?
  - The GNOME3 Desktop Environment
  - What is Shell?
  - Working with Command Line

- **File and Directory Management**
  - Linux Filesystem Hierarchy
  - Create, Delete, and Manage Directories & Files
  - Managing Files with Shell Expansion

- **Getting Help and Documentation**
  - Getting Help for Commands Usage
  - Documentation Using `man` Command
  - Documentation Using `pinfo` Command
  - Reading Documentation in `/usr/share/doc`

- **Standard I/O and Vim Text Editor**
  - Redirecting Output to a File or Program
  - Copying Text Between Windows
  - Standard Input, Output, and Error
  - PIPE, Tee
  - Editing Files with Vim

- **User and Group Management**
  - Linux User Types
  - Gaining Superuser Access
  - Running Commands as Root
  - Creating/Deleting Users and Groups
  - Managing Groups for Authorized Access
  - The Encrypted Passwords for Linux Users
  - `sudoer` and Custom Sudo
  - Controlling User Age

- **File System Permissions**
  - How Linux Permission Works?
  - Interpreting Files and Directory Permissions
  - Controlling Ownership for Files & Directories
  - Managing File Security
  - Special Permissions
  - Default Permissions and File Access

- **Process Management**
  - What is a Linux Process?
  - Controlling Jobs
  - Managing Background and Foreground Processes
  - Killing Processes
  - Real-Time Monitoring of Process Activity

- **Service and Daemon Control**
  - Identifying Service Types and How They Work
  - Managing Systemd Units
  - Differences Between `init` and `systemd`
  - Controlling System Services and Daemons

- **OpenSSH Configuration**
  - Accessing the Remote Command Line with SSH
  - Secure Shell Login
  - SSH Key-based Authentication
  - Customizing Secure SSH Configuration

- **Log Analysis and Storage**
  - System Log Architecture
  - Reviewing Syslog Files
  - Finding Events with `journalctl`
  - Creating Custom Log Files
  - Adjusting System Time

- **Networking**
  - Validating Network Configuration
  - Configuring Networking with `nmcli`
  - Editing Network Configuration Files
  - Configuring Host Names and Name Resolution

- **Archiving and Copying Files**
  - Managing Compressed Tar Archives
  - Secure Copy (`scp`) and Rsync
  - Installing and Updating Software Packages
  - Using `yum`, `rpm`, `apt`, and Debian Package Managers

---

## Section 2: Linux Server Administration

### Topics Covered:

- **File System Access**
  - Mounting and Unmounting File Systems
  - Creating Soft and Hard Links
  - Searching Files Using `find` and `locate`

- **Regular Expressions and Grep**
  - Matching Text with Grep Using Regular Expressions
  - Using Grep with Logs

- **Advanced Vim Usage**
  - Vim Workflow and Text Management
  - Copy, Paste, and Register Usage
  - Searching and Replacing Text

- **Task Scheduling**
  - One-Time Tasks with `at`
  - Cron Jobs for Recurring Tasks
  - Managing System Cron Jobs
  - Temporary File Management

- **Process Prioritization**
  - Nice and Renice Concepts
  - Adjusting Process Priority

- **Access Control Lists (ACLs)**
  - Interpreting ACLs on Files and Directories
  - Granting and Limiting Access Using ACLs
  - Default ACLs Concepts

- **Security Enhanced Linux (SELinux)**
  - SELinux Concepts and Modes
  - SELinux Contexts and Booleans

- **Disks, Partitions, and File Systems**
  - File System Concepts for Partitions
  - MBR and GPT Partition Tables
  - Creating Swap Partitions

- **Logical Volume Management (LVM)**
  - Logical Volume Concepts
  - Managing and Extending Logical Volumes

- **File Servers**
  - NFS Server and Client Setup
  - Samba Server and Client Setup
  - Secure File Server Deployment

- **Troubleshooting Boot Processes**
  - Repairing Boot Issues
  - Resetting Forgotten Root Passwords
  - GRUB2 Bootloader Updates

- **Linux Firewall**
  - Using Netfilter and IPTables
  - Managing Firewall Rules with Firewalld

- **Web Server Configuration**

---

## Section 3: Linux Security

### Topics Covered:

- **Linux OS Security Concepts**
  - File Attributes
  - Is Linux Secure?
  - Understanding Rootkits and Rootkit Hunters

- **Account and Password Security**
  - Advanced Security for SSHD
  - Physical Security Concepts
  - Single User Mode

- **Boot Loader Security**
  - Securing the Boot Loader
  - Recovering Root Passwords

- **Disk Encryption**
  - Encrypting Disks with LUKS

- **Advanced Security Techniques**
  - Disabling Ctrl+Alt+Delete
  - Using TCP Wrappers
  - Network Scanning with `nmap` and `netcat`

---
