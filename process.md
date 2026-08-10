# 🐧 Process Management Utilities

## 📌 Project Title

**Process Management and Process Manager Utilities — Assignment 6**

---

## 📝 Project Description

This project contains process management utilities developed using Bash Shell Scripting.

The assignment is divided into three parts.

### 🅰️ Part A — otProcessManager

`otProcessManager` is a command-line utility used to monitor and manage Linux processes.

It can find processes using CPU and memory usage, display process duration, find orphan and zombie processes, kill processes, and list processes waiting for resources.

### 🅱️ Part B — ProcessManager

`ProcessManager.sh` is a service management utility that can register scripts as services, start and stop them, check their status, change their priority, and display service details.

### 🅲 Part C — Process Experiments

Part C demonstrates practical Linux process behavior such as clearing a log file, deleting a log file while its process is running, and changing process priority.

---

## 🎯 Objective

The main objectives of this assignment are:

- 🐧 Understand Linux process management.
- 📊 Monitor CPU and memory usage.
- 🔝 Find top processes.
- ⏱️ Find the running duration of processes.
- 👻 Identify orphan processes.
- 🧟 Identify zombie processes.
- 💀 Kill processes by name or PID.
- ⏳ Identify processes waiting for resources.
- ⚙️ Create a process/service manager.
- ▶️ Start and stop background services.
- 📊 Check service status.
- ⚡ Change process priority.
- 🧪 Understand Linux file and process behavior.

---

## ✨ Features

### 🅰️ otProcessManager

- 🔝 Top N processes by memory.
- 🔝 Top N processes by CPU.
- 🐌 Kill the least-priority process.
- ⏱️ Find process running duration by name or PID.
- 👻 List orphan processes.
- 🧟 List zombie processes.
- 💀 Kill a process by name or PID.
- ⏳ List processes waiting for resources.

### 🅱️ ProcessManager

- ➕ Register a service.
- ▶️ Start a service.
- 📊 Show service status.
- 🛑 Stop a service.
- ⚡ Change service priority.
- 📋 List registered services.
- 🔍 Show service details.
- 🆔 Display service PID.
- 📜 Store service logs.

### 🅲 Process Experiments

- 🧹 Clear the log file of a running process.
- 🗑️ Delete the log file of a running process.
- ⚡ Change the priority of a running process.

---

## 🛠️ Tech Stack

- 🐧 Linux
- 🐚 Bash Shell Scripting
- 💻 Linux Command Line

### Linux Commands Used

```text
ps
awk
grep
pgrep
kill
nice
renice
nohup
sleep
cat
echo
rm
mkdir
touch
date
head
