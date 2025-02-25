<div align="center">

# AI_DEBUG v0.0.2

A Comprehensive AI-Powered Command-Line Interface for Programming Assistance,  
Error Debugging, and Command Translation.

<a href="https://app.commanddash.io/agent/github_datavorous_comandi"><img src="https://img.shields.io/badge/AI-Code%20Agent-EB9FDA"></a>
![Python version](https://img.shields.io/badge/python-3.10%2B-blue) <br>

</div>

## Demo

<div align="center"> 

<img src="https://raw.githubusercontent.com/datavorous/comandi/main/imgs/syntax.gif" alt="demo" width="93%">  
   <br>
</div>

## Overview

AI_DEBUG is an AI-driven command-line tool designed to streamline programming workflows by translating natural language instructions into executable shell commands, debugging code, and offering targeted programming assistance. It leverages advanced natural language processing to enhance developer productivity directly from the terminal, using MetaAI(Llama3).

## Features

- **Command Translation:** Converts natural language commands into shell instructions, with the option to execute them directly.
- **Code Analysis:** Supports understanding, debugging, and fixing code files. The tool provides summaries, debugging tips, and suggested code improvements.

## Installation

To install AI_DEBUG, ensure Python 3.10 or higher is installed, and follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/datavorous/AI_DEBUG.git
   cd AI_DEBUG
   ```

2. **Build the package:**
   ```bash
   pip install setuptools wheel
   python setup.py sdist bdist_wheel
   ```

3. **Install the package:**
   ```bash
   pip install .
   ```

4. **Run AI_DEBUG:**
   ```bash
   AI_DEBUG -run
   ```

## Usage

AI_DEBUG supports various functionalities tailored to enhance command-line operations and programming tasks:

1. **Command Execution:**
   - Input a natural language instruction.
   - AI_DEBUG translates it into a shell command, provides a description, and prompts for execution.

2. **Code Analysis:**
   - To analyze code, use:
     ```bash
     understand path/to/file.py
     debug path/to/file.py
     fix path/to/file.py
     ```
   - Specify line ranges for focused analysis:
     ```bash
     understand path/to/file.py:10-15,27-48
     ```

3. **System Information:**
   - AI_DEBUG displays key system details at startup, providing context for further operations.

4. **Interactive Prompts:**
   - Engage with the AI to receive hints, command suggestions, and code fixes. Example:
     ```bash
     :: How do I sort a list in Python?
     ```

## Technical Overview

- **Programming Language:** Python 3.10+
- **Core Libraries:**
  - `rich`: Provides enhanced terminal formatting.
  - `subprocess`: Facilitates command execution.
  - `pkg_resources`: Manages resource paths and dependencies.
  - `MetaAI`: Powers AI-driven features.

## Roadmap

- **User Preferences:** Customizable settings for user-specific preferences.
- **Command History:** Save and recall previous commands.
- **Version Control Integration:** Git and other VCS operations from the CLI.

## Contribution

Contributions are welcome. Please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines.

## License

This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

Special thanks to the creators of the `MetaAI` and `rich` libraries for their invaluable tools.
