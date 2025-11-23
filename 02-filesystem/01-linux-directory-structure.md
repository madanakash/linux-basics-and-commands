# Linux Directory Structure

Linux uses a **hierarchical filesystem** that starts from the root directory `/`.  
Every file and folder exists inside this single tree structure.

Below are the most important directories you must know as a DevOps engineer:

---

## `/` – Root Directory  
The top-level directory. Everything begins here.

---

## `/home` – User Home Directories  
Contains personal folders for all users.  
Example: `/home/akash`

Each user stores:
- Documents  
- Downloads  
- Config files  

---

## `/root` – Root User Home  
Home directory of the **superuser (administrator)**.

---

## `/bin` – Essential User Commands  
Contains basic commands needed for normal system use.

Examples:
- `ls`
- `cp`
- `mv`
- `cat`
- `echo`

---

## `/sbin` – System Administration Commands  
Commands used by superusers for system management.

Examples:
- `shutdown`
- `reboot`
- `fdisk`

---

## `/etc` – Configuration Files  
Stores system-wide config files.

Examples:
- Network configs  
- System services configs  
- `/etc/ssh/sshd_config`

---

## `/var` – Variable Files  
Data that changes often.

Contains:
- Logs → `/var/log`
- Cache  
- Temporary run files  
- Mail queues

---

## `/usr` – User Programs and Utilities  
Stores most installed software and libraries.

Important subdirectories:
- `/usr/bin` → Application binaries  
- `/usr/sbin` → Admin binaries  
- `/usr/lib` → Libraries  

---

## `/tmp` – Temporary Files  
Used by applications to store temporary data.  
Often cleared automatically on reboot.

---

## `/opt` – Optional Software  
Used for manually installed software packages.

---

## `/mnt` and `/media` – Mount Points  
Used for mounting storage devices:
- USB drives  
- External hard disks  
- Network storage  

---

## 🧠 Summary  
The Linux filesystem is organized for:
- Security  
- Reliability  
- Separation of user data and system data  
- Ease of maintenance  
