# **Essential Linux Commands Guide**

## 🚀 **1. `mkdir` - Make Directory**
The `mkdir` command creates new directories in the filesystem.

### **🛠 Usage:**
```bash
mkdir [options] directory_name
```

### **🔹 Common Options:**
- `-p` → Creates parent directories if they don’t exist.
- `-v` → Displays a message for each directory created.

### **📌 Examples:**
- Create a single directory:
  ```bash
  mkdir my_directory
  ```
- Create multiple directories at once:
  ```bash
  mkdir dir1 dir2 dir3
  ```
- Create a directory with parent directories:
  ```bash
  mkdir -p /home/user/new_folder/sub_folder
  ```

---

## ✨ **2. `touch` - Create or Update Files**
The `touch` command creates an empty file or updates the timestamp of an existing file.

### **🛠 Usage:**
```bash
touch [options] file_name
```

### **🔹 Common Options:**
- `-c` → Do not create files, only update timestamps.
- `-t` → Set a custom timestamp.

### **📌 Examples:**
- Create an empty file:
  ```bash
  touch myfile.txt
  ```
- Update the timestamp of an existing file:
  ```bash
  touch myfile.txt
  ```
- Create multiple files at once:
  ```bash
  touch file1.txt file2.txt
  ```

---

## 📝 **3. `nano` - Command-Line Text Editor**
`nano` is a simple text editor used for editing files.

### **🛠 Usage:**
```bash
nano [options] file_name
```

### **🔹 Common Commands Inside `nano`:**
- `CTRL + O` → Save the file.
- `CTRL + X` → Exit `nano`.
- `CTRL + K` → Cut text.
- `CTRL + U` → Paste text.

### **📌 Examples:**
- Open a file for editing:
  ```bash
  nano myfile.txt
  ```
- Open a file in read-only mode:
  ```bash
  nano -v myfile.txt
  ```

---

## 📜 **4. `cat` - Display File Contents**
The `cat` command displays file contents or concatenates multiple files.

### **🛠 Usage:**
```bash
cat [options] file_name
```

### **🔹 Common Options:**
- `-n` → Number all output lines.
- `-b` → Number only non-blank lines.
- `-E` → Display `$` at the end of each line.

### **📌 Examples:**
- Display file contents:
  ```bash
  cat myfile.txt
  ```
- Concatenate multiple files:
  ```bash
  cat file1.txt file2.txt > combined.txt
  ```
- Display line numbers:
  ```bash
  cat -n myfile.txt
  ```

---

## 📂 **5. `cp` - Copy Files & Directories**
The `cp` command copies files and directories.

### **🛠 Usage:**
```bash
cp [options] source destination
```

### **🔹 Common Options:**
- `-r` → Copy directories recursively.
- `-i` → Prompt before overwriting.
- `-v` → Show details of the operation.

### **📌 Examples:**
- Copy a file:
  ```bash
  cp file1.txt file2.txt
  ```
- Copy a directory and its contents:
  ```bash
  cp -r dir1/ dir2/
  ```

---

## 🔄 **6. `mv` - Move or Rename Files**
The `mv` command moves or renames files and directories.

### **🛠 Usage:**
```bash
mv [options] source destination
```

### **🔹 Common Options:**
- `-i` → Prompt before overwriting.
- `-v` → Show details of the operation.

### **📌 Examples:**
- Rename a file:
  ```bash
  mv oldfile.txt newfile.txt
  ```
- Move a file to a different directory:
  ```bash
  mv file.txt /home/user/Documents/
  ```

---

## ❌ **7. `rm` - Remove Files & Directories**
The `rm` command deletes files and directories.

### **🛠 Usage:**
```bash
rm [options] file_name
```

### **🔹 Common Options:**
- `-i` → Prompt before deleting.
- `-f` → Force delete.
- `-v` → Show details of deleted files.

### **📌 Examples:**
- Remove a file:
  ```bash
  rm myfile.txt
  ```
- Remove a directory and its contents:
  ```bash
  rm -rf mydirectory/
  ```

---

## 🔍 **8. `grep` - Search for Text in Files**
The `grep` command searches for a specified pattern in files.

### **🛠 Usage:**
```bash
grep [options] pattern file_name
```

### **🔹 Common Options:**
- `-i` → Ignore case.
- `-r` → Search recursively.
- `-l` → Show only filenames.
- `-n` → Show line numbers.
- `-v` → Invert match.

### **📌 Examples:**
- Search for a string in a file:
  ```bash
  grep "search_term" myfile.txt
  ```
- Search recursively in a directory:
  ```bash
  grep -r "search_term" /path/to/dir/
  ```

---

## 📂 **9. `cd ..` - Move Up One Directory Level**
The `cd ..` command moves up one level in the directory tree.

### **🛠 Usage:**
```bash
cd ..
```

### **📌 Examples:**
- Move up one directory:
  ```bash
  cd ..
  ```
- Move up and then navigate to another folder:
  ```bash
  cd ..
  cd folder2/
  ```

---

## **📌 Quick Command Reference:**
| Command | Description | Example |
|---------|-------------|-------------|
| `mkdir` | Create a directory | `mkdir mydir` |
| `touch` | Create an empty file | `touch file.txt` |
| `nano` | Open a text editor | `nano file.txt` |
| `cat` | Display file contents | `cat file.txt` |
| `cp` | Copy files or directories | `cp file1.txt backup/` |
| `mv` | Move or rename files | `mv old.txt new.txt` |
| `rm` | Remove files | `rm file.txt` |
| `rm -r` | Remove directories | `rm -r myfolder/` |
| `grep` | Search for a string in files | `grep "pattern" file.txt` |
| `cd ..` | Move up a directory | `cd ..` |

🚀 **Master these Linux commands to boost your productivity!**

