⭐ Assignment 2
📌 Overview
This assignment builds a UserManager utility that simulates Linux user & group (team) management with proper permission handling:
➜ NinjaTeam Management (Simulate Group)
➜ User Management (Simulate User) under a Team
➜ Shared Directory Structure with Access Control (team & ninja)
➜ Additional Features (change shell, change password, delete user/team, list users/teams)

🎯 Objective
Create a shell script UserManager.sh that simulates adding teams (groups) and users, enforces home directory permission constraints, creates shared team/ninja directories inside every user's home, and supports additional user-management operations.

▶ Usage
./UserManager.sh <operation> <name> <team/shell/args>

📥 Inputs
Symbol	Description
🏷️	Team name (Simulated Group) ex: team1, amigo, unixkings
👤	User name ex: Rakesh, Sandeep, Nitish
🔐	Extra argument (shell path / new password, depending on operation)

📋 Permission Constraints
Rule	Description
🔒 Owner	A user has read, write, execute (rwx) access to their own home directory
👥 Team Members	Fellow team members get read + execute (r-x) access to a user's home directory
🌍 Others	Everyone else gets only execute (--x) access to a user's home directory
📁 team folder	Shared directory inside every home dir — full access (rwx) to same-team members only
📁 ninja folder	Shared directory inside every home dir — full access (rwx) to all ninjas (all users)

📋 Core Operations
Operation	Description	Example
addTeam	Creates a new team (simulated group)	./UserManager.sh addTeam amigo
addUser	Adds a user under a team, sets up home dir + permissions + team/ninja folders	./UserManager.sh addUser Rakesh amigo
delTeam	Deletes a team	./UserManager.sh delTeam amigo
delUser	Deletes a user	./UserManager.sh delUser Rakesh
changePasswd	Changes a user's password	./UserManager.sh changePasswd Rakesh
changeShell	Changes a user's login shell	./UserManager.sh changeShell Rakesh /bin/bash
ls User	Lists all users	./UserManager.sh ls User
ls Team	Lists all teams	./UserManager.sh ls Team

📤 Sample Outputs

⭐ Adding Teams & Users
```
$ ./UserManager.sh addTeam amigo
Team 'amigo' created

$ ./UserManager.sh addTeam unixkings
Team 'unixkings' created

$ ./UserManager.sh addUser Rakesh amigo
User 'Rakesh' added to team 'amigo'

$ ./UserManager.sh addUser Sandeep unixkings
User 'Sandeep' added to team 'unixkings'
```
<!-- 📸 PASTE SCREENSHOT LINK HERE (addTeam, addUser) -->

⭐ Resultant Home Directory Structure
```
$ ls -la /home/Rakesh
drwxr-x--x  4 Rakesh amigo     4096 home
drwxrwx---  2 Rakesh amigo     4096 team
drwxrwx---  2 Rakesh ninja     4096 ninja

$ ls -la /home/Sandeep
drwxr-x--x  4 Sandeep unixkings 4096 home
drwxrwx---  2 Sandeep unixkings 4096 team
drwxrwx---  2 Sandeep ninja     4096 ninja
```
<!-- 📸 PASTE SCREENSHOT LINK HERE (home directory structure & permissions) -->

⭐ Additional Features
```
$ ./UserManager.sh changePasswd Rakesh
Password updated for 'Rakesh'

$ ./UserManager.sh changeShell Rakesh /bin/bash
Shell updated for 'Rakesh'

$ ./UserManager.sh ls User
Rakesh
Sandeep

$ ./UserManager.sh ls Team
amigo
unixkings
```
<!-- 📸 PASTE SCREENSHOT LINK HERE (changePasswd, changeShell, ls User, ls Team) -->

⭐ Deleting User & Team
```
$ ./UserManager.sh delUser Rakesh
User 'Rakesh' deleted

$ ./UserManager.sh delTeam amigo
Team 'amigo' deleted
```
<!-- 📸 PASTE SCREENSHOT LINK HERE (delUser, delTeam) -->

🛠 Concepts Used
✔ Command Line Arguments
✔ case Statement (operation dispatch)
✔ User & Group Management (useradd/adduser, groupadd, userdel, groupdel)
✔ Password & Shell Management (passwd, chsh/usermod -s)
✔ File Permissions (chmod)
✔ Ownership Management (chown, chgrp)
✔ Shared Directory Creation (mkdir)
✔ Listing Users/Groups (cut, /etc/passwd, /etc/group)
✔ Conditional Statements

⚙️ Make Script Executable
chmod +x UserManager.sh

▶ Execute
./UserManager.sh addTeam amigo
./UserManager.sh addUser Rakesh amigo

📁 Assignment
 ├── Problem Statement.txt
 ├── UserManager.sh
 └── README.md

✅ Learning Outcomes
✓ Linux User & Group Administration
✓ Home Directory Permission Design (owner/group/others)
✓ Shared Directory Access Control (team vs ninja scope)
✓ Command Line Argument Handling
✓ case Statement for Operation Dispatch
✓ Password & Shell Management Commands
✓ Listing & Deleting Users/Groups
✓ Script Execution Permissions

🎉 Assignment Completed
