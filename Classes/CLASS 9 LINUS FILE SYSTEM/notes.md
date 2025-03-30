**🖥️ Linux File System Notes**

---

## 📌 1. Introduction to Linux File System
- The Linux file system follows a **hierarchical structure**, with everything under a single root (`/`).
- It adheres to the **Filesystem Hierarchy Standard (FHS)**, ensuring consistency across different Linux distributions.
- **Everything is treated as a file**, including hardware devices.

---

## 📂 2. Linux File System Structure
📁 **`/` (Root Directory)** – The top-level directory containing all other directories.
📁 **`/bin` (Binaries)** – Essential commands like `ls`, `cp`, `mv`.
📁 **`/sbin` (System Binaries)** – System administration commands.
📁 **`/etc` (Configuration Files)** – Stores system configuration files.
📁 **`/home` (User Directories)** – Personal directories for users.
📁 **`/var` (Variable Data)** – Logs, spool files, temporary data.
📁 **`/tmp` (Temporary Files)** – Stores temporary files, cleared on reboot.
📁 **`/usr` (User Programs)** – Holds system-wide installed applications.
📁 **`/opt` (Optional Software)** – Third-party software installations.
📁 **`/mnt` (Mount Directory)** – Used for mounting external file systems.
📁 **`/dev` (Device Files)** – Represents hardware components as files.
📁 **`/proc` (Process Information)** – Virtual file system with process details.
📁 **`/sys` (System Information)** – Contains kernel and hardware details.
📁 **`/boot` (Boot Files)** – Holds bootloader files and kernel images.

---

## 🛠️ 3. Linux File System Types
- 🔹 **Ext4 (Fourth Extended Filesystem)** – Default for most Linux distributions, supports journaling.
- 🔹 **XFS** – High-performance journaling file system.
- 🔹 **Btrfs (B-Tree File System)** – Supports snapshots and advanced features.
- 🔹 **FAT32** – Compatible with Windows, used for USB drives.
- 🔹 **NTFS** – Windows file system, supported via `ntfs-3g`.
- 🔹 **Swap** – Used as virtual memory.

---

## 📜 4. File System Commands
🖥️ **Navigation & Management:**
- `ls` – List directory contents.
- `cd` – Change directory.
- `pwd` – Show current directory.
- `mkdir` – Create a new directory.
- `rm` – Remove files or directories.
- `cp` – Copy files or directories.
- `mv` – Move or rename files.
- `find` – Search for files.

🖥️ **Disk & File System Checks:**
- `df -h` – Display disk usage.
- `du -sh` – Show directory size.
- `mount` – Mount a file system.
- `umount` – Unmount a file system.
- `fsck` – Check and repair file system.

---

## 🔑 5. File System Permissions
- **File Permissions:** `Read (r)`, `Write (w)`, `Execute (x)`
- **User Groups:** `Owner`, `Group`, `Others`
- **Change Permissions:** `chmod` command
- **Change Ownership:** `chown` command
- **Change Group:** `chgrp` command

---

## 🗂️ 6. File System Management
🔹 **Creating a File System:** `mkfs.ext4 /dev/sdx`
🔹 **Checking File System:** `fsck /dev/sdx`
🔹 **Resizing File System:** `resize2fs /dev/sdx`
🔹 **Mounting File System:** `mount /dev/sdx /mnt`
🔹 **Unmounting File System:** `umount /mnt`
🔹 **Checking Disk Usage:** `df -h`
🔹 **Checking Directory Size:** `du -sh`

---

## 📑 7. Special File Types
📂 **Regular Files (-):** Normal files.
📂 **Directory (d):** Contains files and directories.
📂 **Symbolic Links (l):** Shortcut to another file.
📂 **Block Devices (b):** Represents devices like hard disks.
📂 **Character Devices (c):** Represents devices like terminals.
📂 **Sockets (s):** Used for inter-process communication.
📂 **Named Pipes (p):** Used for process communication.

---

## 📌 8. Logical Volume Management (LVM)
- **LVM Components:** Physical Volume (PV), Volume Group (VG), Logical Volume (LV)
- 🔹 **Create Physical Volume:** `pvcreate /dev/sdx`
- 🔹 **Create Volume Group:** `vgcreate my_vg /dev/sdx`
- 🔹 **Create Logical Volume:** `lvcreate -L 10G -n my_lv my_vg`
- 🔹 **Format LV:** `mkfs.ext4 /dev/my_vg/my_lv`
- 🔹 **Mount LV:** `mount /dev/my_vg/my_lv /mnt`
- 🔹 **Resize LV:** `lvextend -L +5G /dev/my_vg/my_lv`

---

## 🛡️ 9. File System Backups
- 📦 **Tar Backup:** `tar -cvf backup.tar /path/to/backup`
- 📦 **Tar Restore:** `tar -xvf backup.tar`
- 📦 **RSYNC Backup:** `rsync -av /source /destination`
- 📦 **DD Image Backup:** `dd if=/dev/sdx of=/backup.img`

---

## 🎯 10. Conclusion
✅ Understanding the Linux file system is crucial for **efficient system administration**.
✅ Proper file system management ensures **storage efficiency, security, and performance**.

