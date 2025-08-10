# **Linux Terminal Cheat Sheet (Mint XFCE)**

A quick translation of common Windows CMD commands into their Linux terminal equivalents.

## **Help**

* **`man [command]`** – Show the manual page for a command.
* **`[command] --help`** – Show basic help for a command.
* **`apropos [keyword]`** – Search for commands related to a keyword.

## **Basic Navigation**

* **`cd [directory]`** – Change the current directory.
* **`TAB`** – Autocomplete file/folder names. Press twice for a list.
* **`cd ..`** – Go up one directory level.
* **`xdg-open [file]`** – Open a file with the default program.
* **`xdg-open [directory]`** – Open file manager in that directory.
* **`xdg-open .`** – Open file manager in the current directory.
* **`ls`** – List files and directories.

  * **`ls -l`** – Detailed list.
  * **`ls -a`** – Show hidden files.
  * **`ls -lh`** – Human-readable sizes.
* **`tree`** – Show folder tree (needs `sudo apt install tree`).

  * **`tree -f`** – Show full paths of all files.
* **`clear`** – Clear the terminal.

## **File and Directory Management**

* **`mkdir [directory]`** – Create a new directory.
* **`rmdir [directory]`** – Remove an empty directory.
* **`rm -r [directory]`** – Remove directory and its contents.

  * **`-f`** – Force removal (no prompt).
* **`rm [file]`** – Delete a file.

  * **`-f`** – Force delete.
  * **`-r`** – Delete recursively (folders).
* **`cp [source] [destination]`** – Copy files or folders.

  * **`-r`** – Copy recursively.
  * **`-u`** – Copy only if newer.
* **`mv [source] [destination]`** – Move or rename files/folders.
* **`rename 's/old/new/' *`** – Batch rename (or `mv oldname newname` for single).

## **System Information**

* **`echo [message]`** – Display a message.
* **`echo $PATH`** – Show the system PATH.
* **`ip addr`** – Show IP configuration.
* **`ip route`** – Show routing table.
* **`sudo dhclient -r`** – Release IP.
* **`sudo dhclient`** – Renew IP.
* **`uname -a`** – Show kernel and OS details.
* **`lsb_release -a`** – Show distribution info.
* **`neofetch`** – Pretty system info (install with `sudo apt install neofetch`).

## **Disk Management**

* **`df -h`** – Show disk usage.
* **`du -sh [path]`** – Show size of a folder/file.
* **`fsck [device]`** – Check disk for errors (`sudo` required, unmount first).
* **`lsblk`** – List storage devices.
* **`parted`** or **`fdisk`** – Partition management tools.
* **`mkfs.ext4 [device]`** – Format a disk to ext4 (careful!).

## **Network Commands**

* **`ping [host]`** – Check network connectivity.
* **`traceroute [host]`** – Trace route to a host (`sudo apt install traceroute`).
* **`netstat -tulnp`** – Show network connections (install with `sudo apt install net-tools`).
* **`ss -tulnp`** – Modern alternative to netstat.

## **Process and Task Management**

* **`ps aux`** – List processes.
* **`top`** – Interactive process monitor.
* **`htop`** – Better process monitor (install with `sudo apt install htop`).
* **`kill [PID]`** – Terminate a process by PID.
* **`kill -9 [PID]`** – Force kill.
* **`pkill [name]`** – Kill processes by name.

## **File Compression**

* **`gzip [file]`** – Compress a file to `.gz`.
* **`gunzip [file.gz]`** – Decompress `.gz` file.
* **`tar -czf archive.tar.gz [folder]`** – Create a `.tar.gz` archive.
* **`tar -xzf archive.tar.gz`** – Extract a `.tar.gz` archive.
* **`zip archive.zip file1 file2`** – Create a `.zip` file.
* **`unzip archive.zip`** – Extract `.zip` file.

## **Miscellaneous**

* **`shutdown now`** – Shutdown immediately.
* **`reboot`** – Restart.
* **`shutdown +5`** – Shutdown in 5 minutes.
* **`xdg-mime query filetype [file]`** – Show file association.
* **`diff [file1] [file2]`** – Compare two files.

## **Keyboard Shortcuts (XFCE Terminal)**

* **`Shift`+`PgUp`** – Scroll up.
* **`Shift`+`PgDn`** – Scroll down.
* **`Ctrl`+`Shift`+`C`** – Copy.
* **`Ctrl`+`Shift`+`V`** – Paste.
* **`Ctrl`+`L`** – Clear screen (like `clear`).
