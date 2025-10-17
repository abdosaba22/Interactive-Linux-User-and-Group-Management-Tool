# 🐧 Interactive Linux User & Group Management Tool (Bash Script)

## ✨ Project Overview

This project is an advanced **Bash shell script** designed to simplify common system administration tasks related to user and group management on Linux systems. It features a fully interactive, menu-driven interface built using the **`whiptail`** utility, making complex `useradd`, `usermod`, `groupadd`, and `groupdel` commands accessible via user-friendly dialog boxes.

The tool ensures all required and optional parameters (like Home Directory, UID, Comment, and Group) are collected robustly before execution.

---

## 🎯 Features

The script provides a comprehensive main menu covering the following actions:

### User Management
* **Add User**: Creates a new user with optional inputs for Home Directory, Comment, UID, and Group.
* **Modify User**: Allows modification of user properties (Comment, Primary Group, Home Directory, UID).
* **Delete User**: Permanently removes a user and their home directory after confirmation.
* **Disable/Enable User**: Locks (`usermod -L`) or unlocks (`usermod -U`) user accounts.
* **Change Password**: Prompts for a new password using the secure console `passwd` command.
* **List Users**: Displays current users along with their Primary Group IDs.

### Group Management
* **Add Group**: Creates a new group.
* **Modify Group**: Allows renaming the group or adding/removing members.
* **Delete Group**: Removes an existing group after confirmation.
* **List Groups**: Displays groups and their GIDs.

---

## 🛠️ Prerequisites (CentOS/RHEL)

To run this script, you need:

1.  **A CentOS or RHEL environment.**
2.  **`whiptail` utility**: This is required for the interactive menus. On CentOS/RHEL, the `whiptail` utility is typically part of the `newt` package.
    ```bash
    # Install whiptail (part of the 'newt' package) using YUM
    sudo yum install newt -y
    # OR, if you are on CentOS/RHEL 8 or newer, use DNF:
    # sudo dnf install newt -y
    ```
3.  **Superuser (sudo) privileges** to perform user/group modifications.

---

## ⚙️ Installation and Usage

1.  **Clone the Repository:**
    ```bash
    git clone <Insert Your GitHub Repository Link Here>
    cd <repo-name>
    ```

2.  **Make the Main Script Executable:**
    ```bash
    chmod +x main_script.sh
    ```

3.  **Run the Tool:**
    ```bash
    sudo ./main_script.sh
    ```
    *(Note: Running with `sudo` is necessary for the underlying system commands.)*

---

## 👨‍💻 Project Attributions

| Detail | Information |
| :--- | :--- |
| **Course** | ITI Bash Scripting Course |
| **Supervisor** | Eng. Romany |
| **Developer** | **Abdalrahman Amin Sabaa** |
| **Role** | System Admin and DevOps Trainee |
| **Contact Email** | abdalrahmansaba@gmail.com |
| **LinkedIn URL** | [Connect with me on LinkedIn](<Insert Your LinkedIn Profile Link Here>) |
| **GitHub Repo** | [View Source Code](<Insert Your GitHub Repository Link Here>) |
