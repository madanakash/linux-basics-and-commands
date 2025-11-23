# 📂 Linux Navigation Commands

This guide covers essential commands for navigating the Linux filesystem, moving between directories, and efficiently exploring your system.

---

## 1. `pwd` – Print Working Directory

Displays your current directory.

```bash
pwd
# Example output:
/home/user/Documents
```

---

## 2. `ls` – List Directory Contents

Lists files and directories.

```bash
ls           # Simple list
ls -l        # Detailed list (permissions, owner, size, date)
ls -a        # Include hidden files
ls -la       # Detailed + hidden files
```

---

## 3. `cd` – Change Directory

Moves between directories.

```bash
cd /home/akash/Documents   # Go to specific directory
cd ..                      # Move one level back
cd ~                       # Go to home directory
cd -                       # Switch to previous directory
```

---

## 4. `mkdir` – Make Directory

Creates new folders.

```bash
mkdir new_folder           # Create a folder
```

---

## 5. `rmdir` – Remove Directory

Deletes an empty directory.

```bash
rmdir folder_name
```
> **Note:** Use `rm -rf folder_name` to delete directories with content.

---

## 6. `tree` – View Directory Structure

Displays a tree view of files and folders (may require installation).

```bash
tree
tree -L 2  # Limit depth to 2 levels
```

---

## 7. `find` – Search for Files & Directories

Locates files or directories anywhere in the system.

```bash
find /home/user -name "file.txt"
find . -type d -name "project*"
```

---

## 8. `locate` – Quickly Find Files

Performs fast searches using a prebuilt database (requires `mlocate` package).

```bash
locate file.txt
```

---

## ✅ Tips for Linux Navigation

- Use <kbd>Tab</kbd> for auto-completion of file/folder names.
- Use <kbd>Ctrl</kbd> + <kbd>R</kbd> to search previous commands.
- Combine commands with `&&` to execute them sequentially:

```bash
cd ~/Documents && ls -l
```
