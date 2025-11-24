# 🔐 File Permissions & `chmod` — Simple Guide

Linux controls who can **read**, **write**, or **run** files using permissions. Here’s a super simple breakdown:

---

## 1️⃣ What Are File Permissions?

There are **three types** of permissions:

| Symbol | Name    | What it means      |
|--------|---------|--------------------|
| `r`    | Read    | View file contents |
| `w`    | Write   | Edit or delete     |
| `x`    | Execute | Run as a program   |

---

## 2️⃣ Who Gets Permissions?

Each file has permissions for **three groups**:

| Group | Who is it?           | Symbol |
|-------|----------------------|--------|
| User  | File owner           | `u`    |
| Group | Users in same group  | `g`    |
| Others| Everyone else        | `o`    |
| All   | Everyone (`u+g+o`)   | `a`    |

---

## 3️⃣ Permission Numbers (Easy!)

Permissions are shown as numbers:

| Number | Permissions | Meaning           |
|--------|-------------|-------------------|
| 0      | ---         | No access         |
| 1      | --x         | Execute only      |
| 2      | -w-         | Write only        |
| 3      | -wx         | Write + execute   |
| 4      | r--         | Read only         |
| 5      | r-x         | Read + execute    |
| 6      | rw-         | Read + write      |
| 7      | rwx         | All permissions   |

---

## 4️⃣ How to Use `chmod`

The `chmod` command changes permissions.  
Format: `chmod XYZ filename`

- **X** = Owner (user)
- **Y** = Group
- **Z** = Others

**Example:**  
`chmod 755 script.sh`  
Breakdown:
- 7 = rwx (owner: all permissions)
- 5 = r-x (group: read + execute)
- 5 = r-x (others: read + execute)

---

## 5️⃣ Most Useful `chmod` Commands

| What you want to do                | Command              |
|------------------------------------|----------------------|
| Only owner can do everything       | `chmod 700 file`     |
| Make a script executable           | `chmod +x script.sh` |
| Owner can write, others can read   | `chmod 644 notes.txt`|
| Everyone can do everything (unsafe)| `chmod 777 test`     |

---

## 6️⃣ Reading Permissions with `ls -l`

Example output:  
`-rw-r--r--`

| Part   | Who   | Permissions      |
|--------|-------|------------------|
| rw-    | Owner | Read + write     |
| r--    | Group | Read             |
| r--    | Others| Read             |

---

## 7️⃣ Quick Cheat Sheet

- 4 = read
- 2 = write
- 1 = execute
- 7 = rwx (all)
- 6 = rw-
- 5 = r-x
- 0 = ---

Shortcuts:
- `u` = user (owner)
- `g` = group
- `o` = others
- `a` = all

---

## 🎯 Summary

- **7** → everything  
- **6** → read + write  
- **5** → read + execute  
- **4** → read  
- **0** → nothing  
- **Format:** user / group / others

That’s all!
