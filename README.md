# cShell
Basic custom shell in C

Introduction - 
This project implements a custom shell in C. The shell supports running commands with arguments, pipelines, and basic input/output redirection. It works on Linux and macOS environments.

Prerequisites -
C Compiler: Ensure you have GCC or Clang installed.

On Linux: sudo apt-get install gcc (Debian/Ubuntu) or sudo yum install gcc (Red Hat/CentOS).
On macOS: Install Xcode Command Line Tools using xcode-select --install.
Make Utility: Make sure the make command is available.

On Linux: Already installed in most distributions; otherwise, use your package manager.
On macOS: Comes with Xcode Command Line Tools.
Shell Files:

The project consists of three main files:
shell.c
utils.c
utils.h
Installation Steps
Clone the Repository:

Place all provided files (shell.c, utils.c, utils.h) into a project folder.
Navigate to the Folder:

Open a terminal and navigate to the project directory:
cd /path/to/project

Build the Shell:

Run the make command to compile the shell:
make

If make is not available, use GCC manually:
gcc shell.c utils.c -o shell
Usage

Run the Shell:

Execute the shell binary:
./shell

Test Commands:

Use standard shell commands such as:
ls
echo "Hello, World!"
pwd

To use pipelines:
ls | wc
Exit the Shell:

Press Ctrl+C or type exit to close the shell.

Troubleshooting
Common Errors:

Missing Compiler: Install GCC or Clang as mentioned above.
Permission Denied: Run chmod +x shell to make the binary executable.

Debugging:

To debug, add -g to the GCC compilation command:

gcc -g shell.c utils.c -o shell

Validation:

Validate the commands and pipelines using print_pipeline from the utils library.
