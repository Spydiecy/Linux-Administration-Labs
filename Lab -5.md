## Problem: Implement ps, top, kill command with their options.Installing, updating, and removing software by apt-get command. 
---

## A) Process Management Commands

### 1. `ps` Command
The `ps` command is used to view information about processes running on the system.

#### Examples:
```bash
ps          # Lists processes for the current shell
```
![image](https://github.com/user-attachments/assets/01a4aa8c-aa68-4a02-a4cc-7ec9d98b583e)

```
ps -e       # Lists all processes running on the system
```
![image](https://github.com/user-attachments/assets/30de6971-823b-4bfc-a060-614e5db9b85b)

```
ps -f       # Shows processes in full-format listing (details like user, PID, etc.)
```
![image](https://github.com/user-attachments/assets/b6eedd20-7d71-456f-be4c-6acbc7bb9843)

```
ps aux      # Displays all processes with detailed information
```
![image](https://github.com/user-attachments/assets/c467801e-55d1-4b87-9ccb-1ccf78176bd3)

```
ps -ef | grep <process_name>  # Searches for a specific process
```

### 2. `top` Command
The `top` command provides a real-time view of system processes and their resource usage.

#### How to Use:
```bash
top                # Starts the top command
```

#### Key Options (Interactive Usage):
- `k`: Kill a process by entering its PID.
- `h`: Help menu for top.
- `u`: Filter processes by a specific user.
- `q`: Quit the top command.

![image](https://github.com/user-attachments/assets/6f7b0c1f-4af2-4a88-a453-0c23f43c9a83)

### 3. `kill` Command
The `kill` command is used to terminate processes by their PID.

#### Examples:
```bash
ps -e               # Find the PID of a process
kill <PID>          # Kills the process with the given PID
kill -9 <PID>       # Force kills the process
```

#### Options:
- `-9`: Sends the SIGKILL signal to forcefully terminate the process.
- `-15`: Sends the SIGTERM signal to gracefully terminate the process.


## B) Software Management Commands

### 1. Installing Software with `apt-get`
The `apt-get` command is used for managing software packages in Debian-based systems.

#### Installing a Package:
```bash
sudo apt-get update                  # Updates the list of available packages
sudo apt-get install <package_name>  # Installs the specified package
```
![image](https://github.com/user-attachments/assets/9349ec57-e189-41e3-a128-5f50b579f1d7)

### 2. Updating Software with `apt-get`
```bash
sudo apt-get update       # Updates package information
sudo apt-get upgrade       # Installs newer versions of installed packages
```

### 3. Removing Software with `apt-get`
```bash
sudo apt-get remove <package_name>       # Removes the specified package
sudo apt-get purge <package_name>        # Removes the package and its configuration files
```
