<br/>
<p align="center">
  <a href="https://github.com/The-Intruder/Lightweight-Unix-Shell-Implementation-aka-Minishell">
    <img src="https://upload.wikimedia.org/wikipedia/commons/f/f9/Windows_Terminal_Logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Lightweight Unix Shell Implementation <em>(Minishell)</em></h3>

  <p align="center">
    A simplified Unix shell that allows users to interact with the operating system through a command-line interface. It involves implementing features such as command execution, environment variable management, process handling, and input/output redirection. It provides a learning opportunity for understanding system calls, process management, and programming in C.
    <br/>
    <br/>
    <a href="https://github.com/The-Intruder/Lightweight-Unix-Shell-Implementation-aka-Minishell/issues">Report Bug</a>
    .
    <a href="https://github.com/The-Intruder/Lightweight-Unix-Shell-Implementation-aka-Minishell/issues">Request Feature</a>
  </p>
</p>

<div  style="display: flex; justify-content: center;">
<a  href="https://twitter.com/i_am_amine" target="_blank">
  <img  alt="Twitter Follow"  src="https://img.shields.io/twitter/follow/i_am_amine?style=social">
</a>
<img  src="https://img.shields.io/github/repo-size/The-Intruder/Lightweight-Unix-Shell-Implementation-aka-Minishell"  alt="Repo Size">
<img  src="https://img.shields.io/github/last-commit/The-Intruder/Lightweight-Unix-Shell-Implementation-aka-Minishell"  alt="Last Commit">
<img  src="https://img.shields.io/github/license/The-Intruder/Lightweight-Unix-Shell-Implementation-aka-Minishell" alt="License" >
<img  src="https://img.shields.io/badge/Made%20with-❤-1f425f.svg"  alt="made-with-love">
</div>


## Table Of Contents

- [Table Of Contents](#table-of-contents)
- [About The Project](#about-the-project)
- [Built With](#built-with)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Customization and Extension](#customization-and-extension)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
  - [Creating A Pull Request](#creating-a-pull-request)
- [License](#license)
- [Authors](#authors)
- [Acknowledgements](#acknowledgements)

## About The Project

The Minishell project is a fundamental endeavor in system programming and operating systems. It involves the development of a simplified Unix shell, which serves as a command-line interface for users to interact with the operating system. The project aims to provide a basic understanding of how a shell works and the underlying mechanisms involved in command execution, process management, and input/output operations.

In this project, we implemented key functionalities that enable the shell to interpret and execute commands entered by the user. This includes parsing and tokenizing user input to separate commands and their arguments, handling command-line options and parameters, and supporting built-in commands like "cd" for directory navigation and "echo" for printing output.

One of the essential aspects of the Minishell project is process management. It was necessary to create child processes to execute external commands and manage their execution, ensuring proper termination and handling of signals. This involved utilizing system calls such as "fork," "exec," and "wait" to spawn new processes and execute programs within them.

Additionally, the project required the managing of environment variables, which are essential components of a shell. We handled tasks like setting, updating, and retrieving environment variables, allowing users to customize their shell environment according to their needs.

Input/output redirection is another crucial feature that we implemented. The shell supports redirecting standard input and output to and from files, enabling users to manipulate data streams effectively. This pushed us to understand file descriptors and to use system calls like "open," "dup," and "close" to redirect input and output streams.

Throughout the project, proper error handling was crucial. We were able to detect and report errors gracefully, ensuring that the shell provides meaningful error messages to the user in case of invalid commands, file access issues, or other exceptional scenarios.

## Built With

The Minishell project is built using the following technologies and concepts:

- **Programming Language:** The Minishell project is primarily implemented in the C programming language, leveraging its low-level capabilities and direct interaction with system calls and processes.

- **System Calls:** The project extensively utilizes various system calls provided by the operating system, such as `fork`, `exec`, `wait`, `open`, `dup`, and `close`, to manage processes, execute programs, and handle input/output redirection.

- **Process Management:** The shell implements process management functionalities to create child processes, manage their execution, and ensure proper termination. This involves understanding and utilizing concepts like process IDs, signal handling, and the exec family of system calls.

- **Command-line Parsing:** The project incorporates techniques for parsing and tokenizing user input to identify separate commands, arguments, options, and parameters. This includes handling spaces, quotes, and special characters to ensure accurate command interpretation.

- **Environment Variables:** The shell manages environment variables, allowing users to set, update, and retrieve variables that define the shell's environment. This involves utilizing the relevant system calls and data structures to maintain and manipulate environment variables effectively.

- **Input/Output Redirection:** The shell supports input/output redirection, enabling users to redirect standard input and output to and from files. This involves understanding file descriptors and using appropriate system calls to redirect input and output streams as requested by the user.

- **Error Handling:** Proper error handling is implemented throughout the project to detect and report errors gracefully. This ensures that the shell provides meaningful error messages to the user in case of invalid commands, file access issues, or other exceptional scenarios.

- **C Standard Library:** The project utilizes various functions from the C Standard Library to handle string manipulation, memory allocation, file operations, and other common programming tasks.

By combining these technologies, concepts, and programming techniques, the Minishell project provides a functional and efficient shell that allows users to interact with the operating system through a command-line interface.

## Getting Started

To get started with the Minishell project, follow the instructions below:

### Prerequisites

- **Operating System:** The Minishell project is primarily designed for Unix-like operating systems, such as Linux or macOS. Ensure that you have a compatible operating system installed on your machine.

- **C Compiler:** You will need a C compiler to build and run the Minishell project. The most commonly used compiler is GCC (GNU Compiler Collection). Make sure you have GCC or an equivalent C compiler installed.

### Installation

1. **Clone the repository:** Begin by cloning this repository to your local machine using the following command:

```bash
git clone https://github.com/The-Intruder/Lightweight-Unix-Shell-Implementation-aka-Minishell minishell
```

2. **Navigate to the project directory:** Move into the project directory using the following command:

```bash
cd minishell
```

3. **Build the project:** Use the makefile provided in the project to build the Minishell executable by running the following command:

```bash
make
```

4. **Run the Minishell:** Once the project is successfully built, you can run the Minishell by executing the following command:

```bash
./minishell
```

## Usage

- After launching the Minishell, you can start entering commands just like you would in a regular shell. The Minishell supports common commands and features, such as executing external programs, navigating the file system with the `cd` command, displaying output with the `echo` command, and handling input/output redirection.

- You can exit the Minishell by typing the `exit` command or by pressing `Ctrl + D`.

## Customization and Extension

The Minishell project provides a basic foundation for a shell. You can customize and extend it to add additional features based on your requirements. This can include implementing new built-in commands, expanding input/output redirection capabilities, or enhancing the error handling mechanism.

To modify the Minishell project, navigate to the project directory and open the source code files in your preferred text editor. Make the necessary changes, save the files, and rebuild the project using the make command.

## Roadmap

The Minishell project can be approached in multiple stages or milestones. Here's a suggested roadmap that outlines the key components and functionalities you can focus on as you progress:

1. **Basic Shell Setup:**
   - Set up the shell infrastructure, including a main loop to read user input and execute commands.
   - Implement basic command execution by forking a child process and executing the entered command.

2. **Command Parsing and Tokenization:**
   - Implement a command parser to separate the command and its arguments.
   - Tokenize user input to handle spaces, quotes, and special characters properly.

3. **Built-in Commands:**
   - Implement built-in commands like `cd` for changing directories, `echo` for displaying output, and `exit` for exiting the shell.
   - Handle these built-in commands within the shell, without creating separate processes.

4. **External Command Execution:**
   - Enable execution of external commands by creating child processes using the `fork` system call.
   - Use the `exec` family of system calls to replace the child process with the desired command.

5. **Process Management:**
   - Handle process termination, both through normal command completion and by handling signals like `Ctrl+C` and `Ctrl+Z`.
   - Implement features like background execution and process suspension/resumption.

6. **Environment Variables:**
   - Manage environment variables within the shell, including setting, updating, and retrieving variables.
   - Handle environment variables for the shell's own environment and individual processes.

7. **Input/Output Redirection:**
   - Implement input/output redirection by redirecting standard input and output to and from files.
   - Support features like appending output to a file (`>>`), input from a file (`<`), and piping (`|`) between commands.

8. **Error Handling and User Feedback:**
   - Implement proper error handling for various scenarios, such as invalid commands, file access issues, and incorrect syntax.
   - Provide meaningful error messages to guide users and facilitate debugging.

9. **Testing and Refinement:**
   - Test the Minishell thoroughly, covering various command combinations, edge cases, and error scenarios.
   - Refine and optimize the codebase, ensuring proper memory management, code modularity, and efficiency.

This roadmap provides a general progression for building the Minishell project, but feel free to adjust and iterate based on your preferences and project requirements.

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

- If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/The-Intruder/Lightweight-Unix-Shell-Implementation-aka-Minishell/issues/new) to discuss it, or directly create a pull request after you edit the _README.md_ file with necessary changes.
- Please make sure you check your spelling and grammar.
- Create individual PR for each suggestion.

### Creating A Pull Request

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the **GPL-3** License. See [LICENSE](https://github.com/The-Intruder/Lightweight-Unix-Shell-Implementation-aka-Minishell/blob/main/LICENSE.md) for more information.

## Authors

- **Mohamed Amine Naimi** aka ***[The-Intruder](https://github.com/The-Intruder/)*** - _Computer Science Student_ - *Built the **Input Execution** part of the Minishell project*
- **Reda El Fagrouch** aka ***[G44R4](https://github.com/ridaelfagrouch/)*** - _Computer Science Student_ - *Built the **Input Parsing** part of the Minishell project*

## Acknowledgements

- [The-Intruder](https://github.com/The-Intruder/)
- [G44R4](https://github.com/ridaelfagrouch/)
