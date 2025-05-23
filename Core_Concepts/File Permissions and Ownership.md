# 🔐 Linux File Permissions

Linux is a multi-user system, and **file permissions** determine who can read, write, or execute a file.

---

## 📄 Permission Basics

Each file or directory has three types of permissions for **three categories** of users:

| Symbol | Permission Type | Description |
|--------|------------------|-------------|
| `r`    | Read             | View file contents or list directory contents |
| `w`    | Write            | Modify file or directory (create/delete files) |
| `x`    | Execute          | Run the file as a program or access a directory |

---

## 👥 User Categories

| Category | Description |
|----------|-------------|
| `u` (user) | The owner of the file |
| `g` (group) | Users who belong to the file's group |
| `o` (others) | All other users |
| `a` (all) | All categories (u+g+o) |

---

## 🧾 Viewing Permissions

```bash
ls -l # Shows permission for all the files in the given folder

## 🔧 Changing Permissions

chmod – Change Mode (permissions)

## 👑 Changing Ownership

## chown - Change file owner

sudo chown newuser file.txt
sudo chown newuser:newgroup file.txt

## chgrp - Change Group privileges

sudo chgrp devteam project.sh