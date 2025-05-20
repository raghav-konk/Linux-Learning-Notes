# ⚙️ Linux Notes – Processes & Jobs

Understanding how Linux handles processes and jobs is crucial for system management and multitasking from the command line.

---

## 🧠 What is a Process?

A **process** is a program in execution. Each process has:
- A unique PID, usually a number (Process ID)
- Its own memory and environment
- Resources like CPU and file descriptors
- consumes RAM

---

## 🔍 Viewing Processes

### Basic Commands

```bash
ps            # Shows current shell's active processes
ps aux        # Lists all running processes in detail
top           # Live, updating list of processes
htop          # Colorful, interactive version of top (must install)