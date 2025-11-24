# 📂 File & Directory Operations (Create, Delete, Move)

A quick reference for essential Linux file operations.

---
## ✅ 1. Creating Files

### Using `touch`
Create an empty file or update its timestamp:
```bash
touch file.txt
touch notes.log
touch index.html
```

### Using `vim`
Create a file and open it in the Vim editor:
```bash
vim file.txt
```
**Vim basics:**
- `i` → insert mode  
- `Esc` → exit insert mode  
- `:wq` → save and exit  

> I prefer using Vim among all editors.

---

## ✅ 2. Creating Directories

### Basic directory
```bash
mkdir test
```

### Nested directories
```bash
mkdir -p project/src/config
```

---

## ❌ 3. Deleting Files & Directories

### Delete a file
```bash
rm file.txt
```

### Force delete a file (dangerous!)
```bash
rm -f file.txt
```

### Delete a directory
```bash
rm -r foldername
```

### Force delete a directory (very dangerous!)
```bash
rm -rf foldername
```

---

## 🔁 4. Moving & Renaming Files

### Move a file
```bash
mv file.txt /home/akash/Documents/
```

### Rename a file
```bash
mv oldname.txt newname.txt
```

### Move multiple files
```bash
mv file1.txt file2.txt folder/
```

---

## 📦 5. Copying Files & Directories

### Copy a file
```bash
cp file.txt backup.txt
```

### Copy a directory recursively
```bash
cp -r project project-backup
```

---

## 🔍 6. Viewing Files

### View file contents
```bash
cat file.txt
```

### View with scroll
```bash
less file.txt
```

---

## ✏️ 7. Editing Files (Vim)

- **Open:** `vim file.txt`
- **Save & Exit:** `:wq`
- **Exit without saving:** `:q!`