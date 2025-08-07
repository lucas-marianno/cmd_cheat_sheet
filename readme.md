# CMD Cheat Sheet

A cheat sheet with some of the most commonly used commands and options in Command Prompt (cmd):

## Command Prompt (cmd) Cheat Sheet

- **`help`**: Shows the list of available commands.

### Basic navigation

- **`cd [directory]`**: Change the current directory.
- **`cd ..`**: Go up one directory level.
- **`dir`**: List files and directories in the current directory.
- **`cls`**: Clear the screen.
- **`tree`**: shows the current folder tree (folders only).
- **`tree /f`**: shows the current folder tree with all files from all child folders.

### File and Directory Management

- **`mkdir [directory]`**: Create a new directory.
- **`rmdir [directory]`**: Remove an empty directory.
  - **`/S`**: Remove all directories and files in the specified directory in addition to the directory itself.
  - **`/Q`**: Run the command without asking for confirmation.
- **`del [file]`**: Delete one or more files.
  - **`/Q`**: Quiet mode, do not ask for confirmation.
  - **`/F`**: Force deletion of read-only files.
  - **`/S`**: Delete specified files from all subdirectories.
- **`copy [source] [destination]`**: Copy files from one location to another.
  - **`/Y`**: Suppress confirmation prompt when overwriting files.
  - **`/V`**: Verify that new files are written correctly.
- **`move [source] [destination]`**: Move files from one location to another.
  - **`/Y`**: Suppress confirmation prompt when overwriting files.
- **`ren [oldname] [newname]`**: Rename a file or folder.
  
### System Information

- **`echo [message]`**: Display a message on the screen.
- **`echo %PATH%`**: Display the system PATH.
- **`ipconfig`**: Display IP network configuration.
  - **`/all`**: Display full IP configuration information.
  - **`/release`**: Release the current IP address.
  - **`/renew`**: Renew the IP address.
- **`systeminfo`**: Display detailed system information.

### Disk Management

- **`chkdsk [volume]`**: Check a disk for errors.
  - **`/F`**: Fix errors on the disk.
  - **`/R`**: Locate bad sectors and recover readable information.
- **`diskpart`**: Open the disk partition management tool.
- **`format [volume]`**: Format a disk.

### Network Commands

- **`ping [host]`**: Send ICMP echo requests to a host to check network connectivity.
- **`tracert [host]`**: Trace the route packets take to a network host.
- **`netstat`**: Display network connections, routing tables, and interface statistics.
  - **`-a`**: Display all connections and listening ports.
  - **`-b`**: Display the executable involved in creating each connection or listening port.
  - **`-n`**: Display addresses and port numbers in numerical form.

### Process and Task Management

- **`tasklist`**: Display a list of currently running processes.
- **`taskkill /PID [pid]`**: Terminate a process by its PID.
  - **`/F`**: Forcefully terminate the process.
  - **`/IM [image name]`**: Terminate a process by its image name.

### File Compression

- **`compact /C [filename]`**: Compress a file.
- **`compact /U [filename]`**: Uncompress a file.
- **`compact /S:[directory]`**: Compress files within a directory.

### Miscellaneous

- **`shutdown /s`**: Shutdown the computer.
  - **`/r`**: Restart the computer.
  - **`/t [seconds]`**: Set a delay for shutdown/restart.
- **`assoc`**: Display or modify file extension associations.
- **`fc [file1] [file2]`**: Compare two files and display the differences.

### Keyboard Shortcuts
  
- **`ctrl`+`shift`+`arrow_up`**: scroll up
- **`ctrl`+`shift`+`arrow_down`**: scroll down
