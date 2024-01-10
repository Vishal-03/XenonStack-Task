# XenonStack-Task
This repository serves as the central hub for my assignment at XenonStack.

This assessment is designed to evaluate your proficiency in Linux system administration and related skills. As part of this assessment, you will encounter a series of tasks and challenges that test your ability to work with Linux-based systems, command-line utilities, and system configurations.

#Assessment Highlights
Command-Line Proficiency: Demonstrate your command-line skills in navigating the Linux filesystem, managing files and directories, and executing commands efficiently.

System Configuration: Configure and manage various aspects of the Linux system, including users, groups, permissions, and system services.

Scripting and Automation: Showcase your scripting abilities to automate common tasks and streamline system administration workflows.

Troubleshooting: Identify and resolve issues related to system performance, networking, and security.

# internctl - Custom Command Line Utility

`internctl` is a custom command line utility written in Bash that provides various functionalities for managing system information, users, and files. It includes subcommands such as `cpu`, `memory`, `user`, and `file`.

## Features

- Display CPU information (equivalent to lscpu)
- Display memory information (equivalent to free)
- Create a new user
- List all users (with optional sudo-only filter)
- Display information about a file, with options to show file size, permissions, owner, and last modification time

## Usage

### Prerequisites

- Bash shell

### Getting Started

1. Clone the repository:

    ```bash
    git clone https://github.com/vishal-03/XenonStack-Task
    ```

2. Navigate to the project directory:

    ```bash
    cd internctl
    ```

3. Make the script executable:

    ```bash
    chmod +x internctl
    ```

4. Run the script with various subcommands:

    ```bash
    ./internsctl --verison
    ./internsctl --help
    ./internsctl cpu getinfo
    ./internsctl memory getinfo
    ./internsctl user create <username>
    ./internsctl user list
    ./internsctl user list --sudo-only
    ./internsctl file getinfo [options] <file-name>
    ```
Version 
<br>
![version](https://github.com/Vishal-03/XenonStack-Task/assets/75837408/54109d9d-d988-41c0-ad91-756c74d018ed)
<br>
Help
<br>
![help](https://github.com/Vishal-03/XenonStack-Task/assets/75837408/a5cfa97b-3098-444b-82f5-e83456355e1d)
<br>
Man intersctl
<br>
![man](https://github.com/Vishal-03/XenonStack-Task/assets/75837408/b33dd7f6-9d9e-4316-85ff-7989d3925a4b)
<br>
CPU Info
![cpu info](https://github.com/Vishal-03/XenonStack-Task/assets/75837408/f362f17a-2426-4865-a97b-a27d7b5ef144)
<br>
Memory Info
<br>
![Screenshot from 2024-01-10 15-11-13](https://github.com/Vishal-03/XenonStack-Task/assets/75837408/1b05c5f1-9e1d-4402-ba46-a0d2d8690955)
<br>
Create User
<br>
![CreateUser](https://github.com/Vishal-03/XenonStack-Task/assets/75837408/343ed0d9-1361-40ef-a832-b30c8d199002)
<br>
All User List
<br>
![userList](https://github.com/Vishal-03/XenonStack-Task/assets/75837408/306874a0-a968-453d-bcc1-68eee4d6965c)
<br>
Sudo user list
<br>
![sudo-Only](https://github.com/Vishal-03/XenonStack-Task/assets/75837408/1c753ee3-c0c6-444f-99b8-bace58dcf860)
<br>





### Subcommands and Options

- **`cpu getinfo`**: Display CPU information.
- **`memory getinfo`**: Display memory information.
- **`user create <username>`**: Create a new user.
- **`user list [--sudo-only]`**: List all users. Use `--sudo-only` to list users with sudo permissions only.
- **`file getinfo [options] <file-name>`**: Display information about a file. Options include `--size`, `--permissions`, `--owner`, and `--last-modified`.

### Examples

```bash
./internctl user create john_doe
./internctl user list --sudo-only
./internctl file getinfo --size --owner myfile.txt

