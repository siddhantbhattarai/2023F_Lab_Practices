# **Linux Commands: Comprehensive Notes with Exercises**

---

## **1. Hardware Information**
### **Commands & Examples**
1. **CPU Information**:  
   ```bash
   lscpu
   ```
   **Output**: Displays CPU architecture, cores, threads, and more.

2. **Memory Information**:  
   ```bash
   free -h
   ```
   **Output**: Displays free and used memory in human-readable format.

3. **Block Devices**:  
   ```bash
   lsblk
   ```
   **Output**: Lists information about block devices (disks, partitions).

### **Exercise**
1. Run `lscpu` and identify the number of CPU cores.
2. Use `free -h` to determine the total and available memory.

---

## **2. File Operations**
### **Commands & Examples**
1. **Create a Directory**:  
   ```bash
   mkdir test_dir
   ```
   **Example**: Creates a directory named `test_dir`.

2. **Create a File**:  
   ```bash
   touch test_file.txt
   ```
   **Example**: Creates an empty file named `test_file.txt`.

3. **Copy a File**:  
   ```bash
   cp test_file.txt copy_test_file.txt
   ```
   **Example**: Copies `test_file.txt` to `copy_test_file.txt`.

4. **Move/Rename a File**:  
   ```bash
   mv copy_test_file.txt renamed_file.txt
   ```
   **Example**: Renames `copy_test_file.txt` to `renamed_file.txt`.

5. **Delete a File**:  
   ```bash
   rm renamed_file.txt
   ```
   **Example**: Deletes `renamed_file.txt`.

### **Exercise**
1. Create a directory called `exercise_dir` and a file named `example.txt` inside it.
2. Copy `example.txt` to `example_copy.txt`.
3. Rename `example_copy.txt` to `final_example.txt` and delete it.

---

## **3. Searching**
### **Commands & Examples**
1. **Find Files by Name**:  
   ```bash
   find ~ -name "*.txt"
   ```
   **Example**: Searches for all `.txt` files in the home directory.

2. **Search File Content**:  
   ```bash
   grep "Ubuntu" /etc/os-release
   ```
   **Example**: Searches for the word `Ubuntu` in the `/etc/os-release` file.

3. **Locate a File**:  
   ```bash
   locate test_file
   ```
   **Example**: Searches for files with the name `test_file`.

### **Exercise**
1. Find all `.log` files in `/var/log`.
2. Search for the word `error` in `/var/log/syslog`.

---

## **4. Directory Navigation**
### **Commands & Examples**
1. **Print Current Directory**:  
   ```bash
   pwd
   ```
   **Example**: Displays the current directory.

2. **Change Directory**:  
   ```bash
   cd /var/log
   ```
   **Example**: Navigates to the `/var/log` directory.

3. **Return to Home Directory**:  
   ```bash
   cd ~
   ```

4. **Move One Level Up**:  
   ```bash
   cd ..
   ```

### **Exercise**
1. Navigate to `/usr/bin` and list all files.
2. Return to the home directory and print its path.

---

## **5. File Permissions**
### **Commands & Examples**
1. **Change Permissions**:  
   ```bash
   chmod 755 test_file.txt
   ```
   **Example**: Assigns read, write, and execute permissions to the owner, and read and execute permissions to others.

2. **Change Ownership**:  
   ```bash
   sudo chown $USER:$USER test_file.txt
   ```
   **Example**: Changes ownership of `test_file.txt` to the current user.

### **Exercise**
1. Create a file `permission_test.txt` and set its permissions to `rw-r--r--`.
2. Change the owner of `permission_test.txt` to `root`.

---

## **6. File Compression**
### **Commands & Examples**
1. **Compress Files**:  
   ```bash
   tar czf test_archive.tar.gz test_dir
   ```
   **Example**: Creates a `.tar.gz` archive of the `test_dir`.

2. **Decompress Files**:  
   ```bash
   tar xzf test_archive.tar.gz
   ```

### **Exercise**
1. Compress a directory `exercise_dir` into `exercise_archive.tar.gz`.
2. Decompress `exercise_archive.tar.gz` and verify its contents.

---

## **7. Processes**
### **Commands & Examples**
1. **List Processes**:  
   ```bash
   ps aux
   ```
   **Example**: Lists all running processes.

2. **Monitor Processes**:  
   ```bash
   top
   ```
   **Example**: Displays system processes interactively.

3. **Kill a Process**:  
   ```bash
   kill <process_id>
   ```
   **Example**: Terminates a process by its ID.

### **Exercise**
1. Use `ps aux` to find the process ID of `bash`.
2. Start a process (e.g., `ping google.com`), suspend it using `Ctrl+Z`, and resume it in the background using `bg`.

---

## **8. Disk Usage**
### **Commands & Examples**
1. **Check Free Disk Space**:  
   ```bash
   df -h
   ```
   **Example**: Displays free and used disk space in human-readable format.

2. **Check Directory Size**:  
   ```bash
   du -sh ~
   ```
   **Example**: Displays the size of the home directory.

### **Exercise**
1. Use `df -h` to check the available disk space on your system.
2. Find the size of `/var/log`.

---

## **9. Networking**
### **Commands & Examples**
1. **Check Connectivity**:  
   ```bash
   ping google.com
   ```
   **Example**: Sends ICMP packets to `google.com`.

2. **Show Network Interfaces**:  
   ```bash
   ifconfig
   ```
   **Example**: Displays details about network interfaces.

3. **SSH into a Remote Host**:  
   ```bash
   ssh user@remote_host
   ```
   **Example**: Connects to a remote host via SSH.

### **Exercise**
1. Ping `example.com` and verify its response time.
2. Use `ifconfig` to find the IP address of your network interface.

---

## **10. User Management**
### **Commands & Examples**
1. **Add a User**:  
   ```bash
   sudo adduser test_user
   ```
   **Example**: Creates a new user `test_user`.

2. **Change a User's Password**:  
   ```bash
   passwd test_user
   ```

3. **List Logged-in Users**:  
   ```bash
   who
   ```

### **Exercise**
1. Create a user named `student_user` and set its password.
2. List all logged-in users using `who`.

---

These commands and exercises will give you hands-on experience with Linux operations on your Ubuntu system.
