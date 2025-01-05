# cShell

cShell is a custom command-line shell implemented in C, designed to execute basic Unix-like commands with support for arguments, pipelines, and input/output redirection. This project serves as an educational tool to understand shell functionalities and process management in Unix-based systems.


## Introduction

The cShell project demonstrates the implementation of a basic shell environment in C, providing insights into command parsing, process creation, and inter-process communication. It supports executing commands with arguments, chaining commands using pipelines, and redirecting input and output streams.

## Features

- **Command Execution**: Run standard Unix commands with arguments.
- **Pipelines**: Chain multiple commands using the pipe (`|`) operator.
- **Input/Output Redirection**: Redirect input (`<`) and output (`>`) streams.
- **Cross-Platform Compatibility**: Works on Linux and macOS environments.

## Prerequisites

Ensure the following tools are installed on your system:

- **C Compiler**: GCC or Clang.
  - *Linux*: Install via package manager if not already installed.
    - Debian/Ubuntu:
      ```bash
      sudo apt-get install gcc
      ```
    - Red Hat/CentOS:
      ```bash
      sudo yum install gcc
      ```
  - *macOS*: Install Xcode Command Line Tools:
    ```bash
    xcode-select --install
    ```
- **Make Utility**: For building the project.
  - *Linux*: Typically pre-installed; if not, install via package manager.
  - *macOS*: Included with Xcode Command Line Tools.

## Installation

Follow these steps to set up and compile cShell:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/AkashDeore15/cShell.git
   ```
2. **Navigate to the Project Directory**:
   ```bash
   cd cShell
   ```
3. **Build the Shell**:
   - Using `make`:
     ```bash
     make
     ```
   - If `make` is unavailable, compile directly with `gcc`:
     ```bash
     gcc shell.c utils.c -o shell
     ```

## Usage

After successful compilation:

1. **Run cShell**:
   ```bash
   ./shell
   ```
2. **Execute Commands**:
   - Standard commands:
     ```bash
     ls -l
     ```
   - Using pipelines:
     ```bash
     ls | grep '.c'
     ```
   - Input/Output redirection:
     ```bash
     cat < input.txt > output.txt
     ```
3. **Exit the Shell**:
   - Type `exit` or press `Ctrl+D` to terminate the shell session.

## Project Structure

- `shell.c`: Main implementation of the shell, handling command input and execution.
- `utils.c`: Utility functions supporting command parsing and processing.
- `utils.h`: Header file declaring utility functions and macros.

## Contributing

Contributions to enhance cShell are welcome. To contribute:

1. **Fork the Repository**.
2. **Create a New Branch**:
   ```bash
   git checkout -b feature-branch
   ```
3. **Commit Your Changes**:
   ```bash
   git commit -m 'Add new feature'
   ```
4. **Push to the Branch**:
   ```bash
   git push origin feature-branch
   ```
5. **Open a Pull Request**.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
