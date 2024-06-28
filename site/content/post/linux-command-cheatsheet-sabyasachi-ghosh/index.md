---
title: Linux Command Cheatsheet - Sabyasachi Ghosh
date: 2024-06-28T16:14:49.784Z
description: In this Tutorial, i will guide you to get the primary and very
  basic knowledge about the linux command which you should aware of.
image: linux_commands.png
---
## Basic Linux Commands

### Navigation and File Operations

1. **`pwd** - Print Working Directory:`
   - Shows the current directory path you are in.

2. **`ls`** - List Directory Contents:
   - Lists files and directories in the current directory.
   - Example: `ls`, `ls -l` (long listing format), `ls -a` (including hidden files).

3. **`cd`** - Change Directory:
   - Moves you to another directory.
   - Example: `cd /path/to/directory`, `cd ..` (move up one directory), `cd ~` (move to your home directory).

4. **`mkdir`** - Make Directory:
   - Creates a new directory.
   - Example: `mkdir myfolder`.

5. **`rmdir`** - Remove Directory:
   - Deletes an empty directory.
   - Example: `rmdir myfolder`.

6. **`cp`** - Copy:
   - Copies files or directories.
   - Example: `cp file1.txt /path/to/destination`, `cp -r directory1 /path/to/destination` (recursive for directories).

7. **`mv`** - Move (or Rename):
   - Moves files or directories to another location or renames them.
   - Example: `mv file1.txt /path/to/destination`, `mv file1.txt file2.txt` (rename).

8. **`rm`** - Remove:
   - Deletes files or directories.
   - Example: `rm file.txt`, `rm -r directory` (recursive for directories, use with caution).

### Viewing and Editing Files

9. **`cat`** - Concatenate and Display:
   - Displays the content of a file.
   - Example: `cat file.txt`.

10. **`less`** - View File Content:
    - Allows viewing large files one screen at a time.
    - Example: `less file.txt` (use arrow keys to scroll, `q` to quit).

11. **`head`** and **`tail`**:
    - **`head`**: Displays the first few lines of a file.
      - Example: `head file.txt`.
    - **`tail`**: Displays the last few lines of a file.
      - Example: `tail file.txt`.

12. **`nano`** or **`vim`**:
    - Text editors for creating and editing files.
    - **`nano`**: Simple and beginner-friendly.
      - Example: `nano newfile.txt`.
    - **`vim`**: More powerful but has a steeper learning curve.
      - Example: `vim newfile.txt`.

### System Information

13. **`uname`** - Print System Information:
    - Shows basic information about the system.
    - Example: `uname -a` (all information).

14. **`df`** - Disk Free:
    - Displays disk space usage of file systems.
    - Example: `df -h` (human-readable format).

15. **`free`** - Memory Usage:
    - Shows free and used memory in the system.
    - Example: `free -h` (human-readable format).

### Process Management

16. **`ps`** - Process Status:
    - Displays currently running processes.
    - Example: `ps aux` (all processes).

17. **`kill`** - Terminate Processes:
    - Ends a process by its ID (PID).
    - Example: `kill PID`.

18. **`top`** or **`htop`**:
    - Interactive process viewer.
    - **`top`**: Basic, built-in.
      - Example: `top`.
    - **`htop`**: More user-friendly and colorful.
      - Example: `htop` (may need to install with `sudo apt install htop` on Debian-based systems).

### Network

19. **`ping`** - Check Network Connection:
    - Tests connectivity to a server or IP address.
    - Example: `ping google.com`.

20. **`ifconfig`** or **`ip addr`**:
    - Displays network configuration.
    - **`ifconfig`**: Older command, may require installation (`sudo apt install net-tools` on newer systems).
      - Example: `ifconfig`.
    - **`ip addr`**: Newer command.
      - Example: `ip addr`.


### Miscellaneous

21. **`date`** - Display Date and Time:
    - Shows current date and time.
    - Example: `date`.

22. **`echo`** - Display Text:
    - Prints text or variables to the terminal.
    - Example: `echo "Hello, Linux!"`.

23. **`history`** - Command History:
    - Lists previously executed commands.
    - Example: `history`.

### Tips

- Use `Tab` key for auto-completion of file and directory names.
- Use `Ctrl+C` to cancel a command.
- Use `Ctrl+D` to log out of a terminal session.

These are some essential Linux commands to get you started. Practice them in your terminal to become more comfortable with using Linux! 

Best wishes, 

Sabyasachi