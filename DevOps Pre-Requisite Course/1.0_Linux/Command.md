# Linux Commands for DevOps with Examples  

Linux commands form the backbone of system administration and DevOps workflows. Here’s a curated list of essential commands with practical examples:  

---

## 1. **File and Directory Management**  
### Commands:  
1. ls - List files and directories.  
   ```bash
   ls -l        # List in detailed format  
   ls -a        # List hidden files  
    ```
2. cd- Change directories.
   ```bash
    cd /var/log  # Navigate to the /var/log directory
    ```
3. pwd - Print the current working directory.
   ```bash
    pwd          # Outputs the full path of the current directory
    ```
4. mkdir - Create a new directory.
   ```bash
    mkdir devops_files   # Create a directory named devops_files 
    ```
5. rm - Remove files or directories.
   ```bash
    rm example.txt       # Remove a file named example.txt  
    rm -r devops_files   # Remove a directory and its contents
    ```
## 2. **File Viewing and Editing**
### **Commands**:
1. cat - Display the contents of a file.
   ```bash
    cat file.txt          # Show the content of file.txt  
    ```
2. nano or vim - Edit a file.
   ```bash
    nano config.yaml      # Open config.yaml in nano editor  
    vim config.yaml       # Open config.yaml in vim editor
    ```
3. less - View file contents one page at a time.
   ```bash
    less /var/log/syslog  # View the system log file
    ```
## 3. **User and Permission Management**
### **Commands**:
1. adduser - Add a new user.
   ```bash
    sudo adduser devops_user  
   ```
2. passwd - Change a user's password.
   ```bash
     passwd devops_user    # Set or update the password for devops_user
   ```
3. chmod - Change file permissions.
   ```bash
   chmod 755 script.sh   # Assign read, write, and execute permissions
    ```
4. chown - Change ownership of a file.
   ```bash
    sudo chown user:group file.txt
   ```
## 4. **Networking**
### **Commands**:
1. ping - Check network connectivity.
   ```bash
    ping google.com       # Ping Google's server
   ```
2. curl - Transfer data from or to a server.
   ```bash
    curl http://example.com
   ```
3. netstat or ss - Show network connections.
     ```bash
    netstat -tuln         # Show active listening ports  
    ss -tuln              # Alternative for netstat
   ```
## 5. **Process and System Monitoring**
### **Commands**:
1. ps - Display running processes.
   ```bash
    ps aux                # List all processes with detailed info  
   ```
2. top - Monitor system performance.
   ```bash
    top                   # Interactive view of running processes
   ```
3. kill - Terminate a process.
     ```bash
      kill -9 1234          # Force kill process with PID 1234 
     ```
## 6. **Disk and File System Management**
### **Commands**:
1. df - Check disk space usage.
     ```bash
    df -h                 # Display disk space in human-readable format
     ```
2. du - Check directory size.
     ```bash
    du -sh /var           # Display total size of the /var directory  
     ```
3. mount - Mount a filesystem.
     ```bash
    sudo mount /dev/sdb1 /mnt  
     ```
## 7. **Package Management**
### **Commands**:
1. Debian-based systems (e.g., Ubuntu):
     ```bash
    sudo apt update       # Update package lists  
    sudo apt install nginx  # Install Nginx web server
     ```
2. Red Hat-based systems (e.g., CentOS):
     ```bash
    sudo yum install httpd  # Install Apache web server  
     ```
## 8. **Shell Scripting**
Example Script:
1. Automate backups:

     ```bash
    #!/bin/bash  
    tar -czf backup.tar.gz /home/user/data  
    echo "Backup completed!"  
     ```
2. Run the script:

     ```bash
    bash backup.sh  
     ```
## 9. **Log Management**
### **Commands**:
1. View logs:
     ```bash
    tail -f /var/log/syslog  # Continuously monitor the system log 
     ```
2. Filter logs:
     ```bash
    grep "error" /var/log/syslog  
     ```
## Conclusion
Mastering Linux commands is essential for DevOps engineers to manage servers, automate tasks, and troubleshoot systems effectively. Regular practice and hands-on experience will ensure proficiency in these commands.


This file lists essential Linux commands for DevOps professionals, along with examples to provide practical insights. Let me know if you’d like to add more advanced topics!






