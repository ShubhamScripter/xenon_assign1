# XenonStack-Assignments

Description
internsctl is a command-line interface designed to provide various server-related information and perform user management tasks. The CLI is organized into three difficulty levels - Easy, Intermediate, and Advanced.

Installation
To install internsctl, follow these steps:

bash
Copy code
# Clone the repository
git clone https://github.com/your-username/internsctl.git

# Navigate to the project directory
cd internsctl

# Install dependencies
npm install

# Make the CLI globally executable
npm link
Usage
Manual Page
To view the manual page for internsctl, execute:

bash
Copy code
man internsctl
Help
For command-specific help, execute:

bash
Copy code
internsctl --help
Version
To check the version of internsctl, use:

bash
Copy code
internsctl --version
Commands
Part 1 - Easy Level
Get CPU Information
bash
Copy code
internsctl cpu getinfo
Expected Output:
Output similar to the lscpu command.

Get Memory Information
bash
Copy code
internsctl memory getinfo
Expected Output:
Output similar to the free command.

Part 2 - Intermediate Level
Create a New User
bash
Copy code
internsctl user create <username>
Note: Creates a user who can log in to the Linux system and access their home directory.

List Users
bash
Copy code
internsctl user list
List Users with Sudo Permissions
bash
Copy code
internsctl user list --sudo-only
Part 3 - Advanced Level
Get File Information
bash
Copy code
internsctl file getinfo <file-name>
Expected Output:
bash
Copy code
File: <file-name>
Access: -rw-r--r--
Size(B): <file-size>
Owner: <file-owner>
Modify: <last-modified-time>
Get Specific File Information
Use options to get specific file information:

--size, -s
bash
Copy code
internsctl file getinfo --size <file-name>
--permissions, -p
bash
Copy code
internsctl file getinfo --permissions <file-name>
--owner, -o
bash
Copy code
internsctl file getinfo --owner <file-name>
--last-modified, -m
bash
Copy code
internsctl file getinfo --last-modified <file-name>
Examples
Example: Get CPU Information
bash
Copy code
internsctl cpu getinfo
Example: Get Memory Information
bash
Copy code
internsctl memory getinfo
Example: Create a New User
bash
Copy code
internsctl user create john_doe
Example: List Users
bash
Copy code
internsctl user list
Example: List Users with Sudo Permissions
bash
Copy code
internsctl user list --sudo-only
Example: Get File Information
bash
Copy code
internsctl file getinfo hello.txt
Example: Get Size of a File
bash
Copy code
internsctl file getinfo --size hello.txt
Example: Get Permissions of a File
bash
Copy code
internsctl file getinfo --permissions hello.txt
Example: Get Owner of a File
bash
Copy code
internsctl file getinfo --owner hello.txt
Example: Get Last Modified Time of a File
bash
Copy code
internsctl file getinfo --last-modified hello.txt
Feel free to explore more commands and options as needed for your server management tasks using internsctl.
