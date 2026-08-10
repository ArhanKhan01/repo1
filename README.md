# ⭐ Assignment 1.2

## 📌 Overview
This assignment focuses on creating a utility script using basic Linux commands to manage directories and files.

→ **FileManager.sh** – A command-line utility for directory and file operations

---

## ⭐ FileManager.sh

### 🎯 Objective
Create a shell script `FileManager.sh` that can perform basic directory and file operations using only simple Linux commands (without using `sed`).

### ✅ Features

#### Directory Operations
- ✔ Create a Directory (`addDir`)
- ✔ Delete a Directory (`deleteDir`)
- ✔ List all content of a Directory (`listAll`)
- ✔ List only files in a Directory (`listFiles`)
- ✔ List only directories in a Directory (`listDirs`)

#### File Operations
- ✔ Create a file (empty or with content) (`addFile`)
- ✔ Add content to a file (`addContentToFile`)
- ✔ Add content at the beginning of a file (`addContentToFileBegining`)
- ✔ Show top n lines of a file (`showFileBeginingContent`)
- ✔ Show last n lines of a file (`showFileEndContent`)
- ✔ Show content of a specific line number (`showFileContentAtLine`)
- ✔ Show content of a specific line range (`showFileContentForLineRange`)
- ✔ Move a file (`moveFile`)
- ✔ Copy a file (`copyFile`)
- ✔ Delete a file (`deleteFile`)
- ✔ Clear file content (`clearFileContent`)

---

### ▶️ Usage
```bash
./FileManager.sh <operation> <path> <name> [extra]
📥 Example Commands
Directory Examples
Bash./FileManager.sh addDir /tmp dir1
./FileManager.sh addDir /tmp dir2
./FileManager.sh addDir /tmp dir3
./FileManager.sh listFiles /tmp
./FileManager.sh listDirs /tmp
./FileManager.sh listAll /tmp
./FileManager.sh deleteDir /tmp dir3
File Examples
Bash./FileManager.sh addFile /tmp/dir1 file1.txt
./FileManager.sh addFile /tmp/dir1 file1.txt "Initial Content"
./FileManager.sh addContentToFile /tmp/dir1 file1.txt "Additional Content"
./FileManager.sh addContentToFileBegining /tmp/dir1 file1.txt "Content at Beginning"
./FileManager.sh showFileBeginingContent /tmp/dir1 file1.txt 5
./FileManager.sh showFileEndContent /tmp/dir1 file1.txt 5
./FileManager.sh showFileContentAtLine /tmp/dir1 file1.txt 2
./FileManager.sh moveFile /tmp/dir1/file1.txt /tmp/dir1/file2.txt
./FileManager.sh copyFile /tmp/dir1/file2.txt /tmp/dir2/
./FileManager.sh deleteFile /tmp/dir1 file2.txt

📤 Sample Outputs
Create Directory
Bash$ ./FileManager.sh addDir /tmp dir1
Directory created
Create File
Bash$ ./FileManager.sh addFile /tmp/dir1 file1.txt "Hello World"
File Created
List All
Bash$ ./FileManager.sh listAll /tmp/dir1
file1.txt
Show File Content
Bash$ ./FileManager.sh showFileBeginingContent /tmp/dir1 file1.txt 5
Hello World
Note: Add your actual terminal screenshots below.

🖼️ Screenshots
(Add your screenshots here)

🛠️ Concepts Used

✔ Command Line Arguments
✔ case statement
✔ Basic Linux Commands (mkdir, rm, ls, find, touch, echo, cat, head, tail, mv, cp)
✔ File and Directory Handling
✔ Conditional Statements


⚙️ Make Script Executable
Bashchmod +x FileManager.sh
▶️ Execute
Bash./FileManager.sh addDir /tmp testdir
./FileManager.sh addFile /tmp/testdir hello.txt "Hello World"
./FileManager.sh listAll /tmp/testdir

📁 Folder Structure
animate-gaussianAssignment-1.2/
├── FileManager.sh
├── README.md
└── screenshots/          # (optional) folder for screenshots
    ├── dir-operations.png
    └── file-operations.png

✅ Learning Outcomes

✔ Bash Scripting
✔ Command Line Arguments
✔ case Statement
✔ Directory Operations using basic commands
✔ File Operations using basic commands
✔ Using head, tail, find, mv, cp etc.
✔ Script Execution Permissions


🎉 Assignment Completed

<img width="1013" height="796" alt="Screenshot 2026-08-09 125425" src="https://github.com/user-attachments/assets/dc2089b1-4e30-45c1-bc83-8ee65671067d" />
<img width="1013" height="796" alt="Screenshot 2026-08-09 125425" src="https://github.com/user-attachments/assets/d6798c15-4762-414a-9474-08412ea2cdcc" />
