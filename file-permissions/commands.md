# 🔐 File Permissions in Linux

Linux uses a **permission system** to control who can read, write, or execute files and directories.  
Permissions apply to:
- **Owner** → The user who owns the file  
- **Group** → Users in the file’s group  
- **Others** → Everyone else  

---

## 👀 Viewing Permissions
| Command | Description |
|---------|-------------|
| `ls -l` | List files with detailed permissions |
| `ls -ld dir/` | Show permissions of a directory itself |
| `stat file` | Show detailed file metadata (including permissions) |

- **Owner:** `rwx` → read, write, execute  
- **Group:** `r-x` → read, execute  
- **Others:** `r--` → read only  

---

## ✏️ Changing Permissions with `chmod`
| Command | Description |
|---------|-------------|
| `chmod 755 file` | Set permissions: rwx (owner), r-x (group), r-x (others) |
| `chmod 644 file` | Set permissions: rw- (owner), r-- (group), r-- (others) |
| `chmod +x script.sh` | Add execute permission |
| `chmod -w notes.txt` | Remove write permission |
| `chmod u+x file` | Add execute for **user (owner)** |
| `chmod g-r file` | Remove read for **group** |
| `chmod o= file` | Remove all permissions for **others** |

---

## 👥 Ownership Management
| Command | Description |
|---------|-------------|
| `chown user file` | Change file owner |
| `chown user:group file` | Change owner and group |
| `chgrp group file` | Change group ownership |

---

## 🔢 Permission Numbers (Octal Notation)
Each permission is represented by a number:
- `r = 4`  
- `w = 2`  
- `x = 1`  

Add them together:
- `7 = rwx`  
- `6 = rw-`  
- `5 = r-x`  
- `4 = r--`  
- `0 = ---`  

➡ Examples:
- `chmod 700 file` → Owner full access, group & others none  
- `chmod 644 file` → Owner read/write, group & others read-only  
- `chmod 755 script.sh` → Everyone can read & execute, only owner can write  

---

## 🛡️ Special Permissions
| Symbol | Octal | Description |
|--------|-------|-------------|
| `s` (setuid) | 4000 | Run file as the **owner** |
| `s` (setgid) | 2000 | Run file as the **group** |
| `t` (sticky bit) | 1000 | Files in directory can only be deleted by their **owner** |

➡ Example:
```bash
chmod 1777 /tmp

