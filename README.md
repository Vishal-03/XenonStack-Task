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
    git clone https://github.com/vishal-03/internctl.git
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
    ./internctl --help
    ./internctl cpu getinfo
    ./internctl memory getinfo
    ./internctl user create <username>
    ./internctl user list
    ./internctl user list --sudo-only
    ./internctl file getinfo [options] <file-name>
    ```

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

