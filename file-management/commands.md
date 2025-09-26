# 📂 File Management Commands in Linux

This section covers the most important Linux commands for **creating, navigating, and managing files & directories**.

---

## 🗂 Directory Management
| Command | Description |
|---------|-------------|
| `pwd` | Show the current working directory |
| `ls` | List files in the current directory |
| `ls -l` | List files with details (permissions, size, owner, etc.) |
| `ls -a` | Show hidden files (those starting with `.`) |
| `cd dir` | Change directory into `dir` |
| `cd ..` | Move up one directory (parent folder) |
| `cd ~` | Go to home directory |
| `mkdir dir` | Create a new directory named `dir` |
| `mkdir -p a/b/c` | Create nested directories in one command |

---

## 📄 File Creation & Viewing
| Command | Description |
|---------|-------------|
| `touch file` | Create an empty file or update timestamp |
| `cat file` | Display the contents of a file |
| `less file` | View file contents one page at a time |
| `head file` | Show the first 10 lines of a file |
| `tail file` | Show the last 10 lines of a file |
| `tail -f file` | Continuously monitor a file (useful for logs) |

---

## ✏️ File Editing
| Command | Description |
|---------|-------------|
| `nano file` | Open file in Nano text editor |
| `vim file` | Open file in Vim text editor |
| `code file` | Open file in VS Code (if installed) |

---

## 📦 File Operations
| Command | Description |
|---------|-------------|
| `cp file dest/` | Copy `file` to `dest/` |
| `cp -r dir dest/` | Copy a directory recursively |
| `mv file dest/` | Move or rename a file |
| `rm file` | Delete a file |
| `rm -r dir/` | Delete a directory and its contents recursively |
| `rm -i file` | Delete a file with confirmation prompt |

---

## 🔍 Searching & Finding Files
| Command | Description |
|---------|-------------|
| `find . -name "file.txt"` | Search for `file.txt` in current directory |
| `grep  "pattern" filename | powerful text search tool |
| `find /path -type d -name "docs"` | Find a directory named "docs" |
| `locate file.txt` | Quickly search for files (requires `updatedb`) |

---

## 📦 Archiving & Compression
| Command | Description |
|---------|-------------|
| `tar -cvf archive.tar dir/` | Create a tar archive of `dir/` |
| `tar -xvf archive.tar` | Extract a tar archive |
| `gzip file` | Compress a file (creates `file.gz`) |
| `gunzip file.gz` | Decompress a `.gz` file |
| `zip archive.zip file` | Create a zip archive |
| `unzip archive.zip` | Extract a zip archive |

---

## ⚡ Useful Shortcuts
- `.` → Current directory  
- `..` → Parent directory  
- `~` → Home directory  
- `*` → Wildcard (matches anything)  

---

✅ With these commands, you can **navigate, create, edit, move, delete, and search** files effectively in Linux.
