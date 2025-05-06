# 📁 Linux File System Notes

The Linux file system is organized as a single inverted tree with the root directory `/` at the top. Everything—files, directories, devices, and even processes—resides under this root.

---

## 📂 Important Directories and Their Purposes

| Directory     | Description |
|---------------|-------------|
| `/`           | Root directory of the entire file system. |
| `/home`       | User home directories (e.g., `/home/user1`) |
| `/bin`        | Essential user binaries (e.g., `ls`, `cp`, `mv`) |
| `/sbin`       | System binaries (e.g., `shutdown`, `mount`) |
| `/etc`        | System-wide configuration files |
| `/var`        | Variable data (e.g., logs, cache, spool) |
| `/tmp`        | Temporary files (cleared on reboot) |
| `/usr`        | User-installed software and libraries |
| `/lib`, `/lib64` | Shared libraries needed for system programs |
| `/dev`        | Device files (e.g., hard drives, USBs) |
| `/proc`, `/sys` | Virtual filesystems for kernel and system process info |
| `/boot`       | Bootloader files including kernels |

---

## 🧠 Use Case Scenario: Troubleshooting a Full Disk

### 🧩 Problem
You're administering a Linux server that suddenly becomes very slow. You suspect a full disk.

### 🛠️ Steps to Troubleshoot

1. **Check disk usage:**
   ```bash
   df -h