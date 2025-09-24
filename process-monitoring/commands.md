# ⚙️ Processes & Monitoring in Linux

Linux is a **multi-tasking OS**, where processes (running programs) can be viewed, monitored, and controlled using commands.  

---

## 👀 Viewing Processes
| Command | Description |
|---------|-------------|
| `ps` | Show processes for the current shell |
| `ps aux` | Show all running processes with details (user, CPU, memory, PID) |
| `ps -ef` | Alternative format for process listing |
| `pgrep process_name` | Find PIDs of processes by name |

---

## 📊 Monitoring in Real Time
| Command | Description |
|---------|-------------|
| `top` | Real-time view of CPU, memory, and processes |
| `htop` | Interactive, user-friendly version of `top` (allows scrolling, filtering, killing) |
| `uptime` | Show system uptime and load averages |
| `free -h` | Show memory (RAM & swap) usage |
| `df -h` | Show disk space usage |
| `du -sh dir/` | Show space used by a directory |
| `iostat` | CPU and disk I/O statistics (needs `sysstat` package) |
| `vmstat` | System memory, process, I/O statistics |
| `sar` | Collect and report system performance data |

---

## 🔧 Managing Processes
| Command | Description |
|---------|-------------|
| `kill PID` | Terminate a process by its PID |
| `kill -9 PID` | Forcefully kill a process |
| `pkill name` | Kill processes by name |
| `jobs` | List background jobs in the current shell |
| `bg %1` | Resume job 1 in the background |
| `fg %1` | Bring job 1 to the foreground |
| `Ctrl+Z` | Suspend a running process |
| `Ctrl+C` | Kill the foreground process |

---

## 📑 Process Identifiers (PID)
- Every process has a **PID** (Process ID)  
- The **init/systemd process** is usually PID 1  
- Use `ps aux` or `pidof` to find a process PID  

---

## 🖥 Example Workflows
🔹 **Find and kill a process**
```bash
ps aux | grep python
kill 1234
