---
title: Linux Command Cheatsheet - Sabyasachi Ghosh
date: 2024-06-28T16:14:49.784Z
description: In this Tutorial, i will guide you to get the primary and very
  basic knowledge about the linux command which you should aware of.
image: linux_commands.png
---
## Why do we need to learn about Linux commands? 


Linux commands are tools used in the terminal to manage files, navigate the system, view system information, control processes, and interact with networks. They are essential for operating and administrating Linux systems efficiently.


### Basic Linux Commands

#### Navigation and File Operations

**`pwd`** - Print Working Directory

   ```bash
   pwd
   ```
   - **Output:** `/home/user`
   - **Explanation:** Prints the current working directory path. Useful when you want to know where you are in the directory structure.

 **`ls`** - List Directory Contents

   ```bash
   ls
   ```
   - **Output:**
     ```
     Desktop  Documents  Downloads  Music  Pictures
     ```
   - **Explanation:** Lists all files and directories in the current directory. Helpful for quickly checking what files are present.

   ```bash
   ls -l
   ```
   - **Output:**
     ```
     total 40
     drwxr-xr-x 2 user user 4096 Jun 28 10:00 Desktop
     drwxr-xr-x 3 user user 4096 Jun 27 14:30 Documents
     drwxr-xr-x 2 user user 4096 Jun 27 12:15 Downloads
     drwxr-xr-x 2 user user 4096 Jun 26 18:00 Music
     drwxr-xr-x 2 user user 4096 Jun 25 09:45 Pictures
     ```
   - **Explanation:** `-l` (long listing) provides detailed information about files and directories, including permissions, owner, size, and last modified date.

   ```bash
   ls -a
   ```
   - **Output:**
     ```
       Desktop  Documents  Downloads  Music  Pictures
     ```
   - **Explanation:** `-a` (all) shows all files and directories, including hidden ones (those starting with `.`).

 **`cd`** - Change Directory

   ```bash
   cd Documents
   ```
   - **Explanation:** Changes the current directory to `Documents`. You can navigate to any directory by specifying its path.

   ```bash
   cd ..
   ```
   - **Explanation:** Moves up one directory level (to the parent directory).

   ```bash
   cd ~
   ```
   - **Explanation:** Changes to the user's home directory (`~` represents the home directory shortcut).

**`mkdir`** - Make Directory

   ```bash
   mkdir myfolder
   ls
   ```
   - **Output:** `myfolder`
   - **Explanation:** Creates a new directory named `myfolder` in the current directory. Use it to organize your files and projects.

**`rmdir`** - Remove Directory

   ```bash
   rmdir myfolder
   ```
   - **Explanation:** Deletes an empty directory named `myfolder`. Use with caution as it cannot remove directories with contents.

**`cp`** - Copy

   ```bash
   echo "Hello, Linux!" > file.txt
   cp file.txt myfolder/
   ls myfolder
   ```
   - **Output:** `file.txt`
   - **Explanation:** Copies `file.txt` from the current directory to `myfolder`. Use `-r` for copying directories and their contents recursively.

**`mv`** - Move (or Rename)

   ```bash
   mv file.txt newfile.txt
   ls
   ```
   - **Output:** `myfolder  newfile.txt`
   - **Explanation:** Renames `file.txt` to `newfile.txt` in the current directory. It can also move files between directories.

**`rm`** - Remove

   ```bash
   rm newfile.txt
   ls
   ```
   - **Output:** `myfolder`
   - **Explanation:** Deletes `newfile.txt` from the current directory. Use `-r` to recursively delete directories and their contents.

#### Viewing and Editing Files

**`cat`** - Concatenate and Display

   ```bash
   cat myfolder/file.txt
   ```
   - **Output:** `Hello, Linux!`
   - **Explanation:** Displays the contents of `file.txt` on the terminal. Useful for reading small files or piping into other commands.

**`less`** - View File Content

    ```bash
    less myfolder/bigfile.log
    ```
    - **Explanation:** Opens `bigfile.log` in a pager that allows scrolling through the file. Use arrow keys to navigate, `q` to quit.

**`head`** and **`tail`** - View File Beginning and End

    ```bash
    head -n 10 myfolder/file.txt
    ```
    - **Output:** First 10 lines of `file.txt`
    - **Explanation:** `head` displays the first few lines of a file. Use `-n` to specify the number of lines.

    ```bash
    tail -n 20 myfolder/bigfile.log
    ```
    - **Output:** Last 20 lines of `bigfile.log`
    - **Explanation:** `tail` displays the last few lines of a file. Useful for monitoring log files or large outputs.

**`nano`** - Text Editor

    ```bash
    nano myfolder/newfile.txt
    ```
    - **Explanation:** Opens `newfile.txt` in the `nano` text editor within the terminal. Use `Ctrl+X` to exit, `Y` to save changes.

#### System Information

**`uname`** - Print System Information

    ```bash
    uname -a
    ```
    - **Output:** `Linux ubuntu 5.4.0-77-generic #86-Ubuntu SMP Thu Jun 17 02:35:03 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux`
    - **Explanation:** Displays detailed information about the system kernel, including version and architecture.

**`df`** - Disk Free

    ```bash
    df -h
    ```
    - **Output:** 
      ```
      Filesystem      Size  Used Avail Use% Mounted on
      /dev/sda1        20G   10G   8G   55% /
      ```
    - **Explanation:** Provides information about disk space usage on mounted filesystems in a human-readable format (`-h`).

#### Process Management

**`ps`** - Process Status

    ```bash
    ps aux
    ```
    - **Output:** 
      ```
      USER       PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
      user      1234  0.0  0.1 225036 13320 ?        Ss   Jun03   0:04 /sbin/init
      ```
    - **Explanation:** Lists all running processes with detailed information such as CPU and memory usage (`aux` for all users).

**`kill`** - Terminate Processes

    ```bash
    kill PID
    ```
    - **Explanation:** Terminates a process identified by its PID (Process ID). Use `ps` to find the PID of the process you want to kill.

#### I hope this cheatsheet helped you. If so, then please share this with your network. Thank you so much!



###### Best Wishes, 

Sabyasachi Ghosh