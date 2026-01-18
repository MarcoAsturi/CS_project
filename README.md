This repository contains analysis and materials related to the exam exercise of Foundation of Computer Science course.

## Python Virtual Environment (venv) Setup Guide

This guide will help you set up a Python virtual environment for this project on Windows, Linux, and macOS.

### Prerequisites

- Python 3.8 or higher installed on your system
- pip (Python package installer)

### Windows

1. **Open Command Prompt or PowerShell**
   - Press `Win + R`, type `cmd` or `powershell`, and press Enter

2. **Navigate to the project directory**
   ```cmd
   cd path\to\CS_project
   ```

3. **Create the virtual environment**
   ```cmd
   python -m venv cs-venv
   ```
   or if you have multiple Python versions:
   ```cmd
   python3 -m venv cs-venv
   ```

4. **Activate the virtual environment**
   ```cmd
   cs-venv\Scripts\activate
   ```
   After activation, you should see `(cs-venv)` at the beginning of your command prompt.

5. **Install required packages**
   ```cmd
   pip install -r requirements.txt
   ```

6. **Deactivate (when done)**
   ```cmd
   deactivate
   ```

### Linux / macOS

1. **Open Terminal**
   - On Linux: Press `Ctrl + Alt + T` or open Terminal from applications
   - On macOS: Press `Cmd + Space`, type "Terminal", and press Enter

2. **Navigate to the project directory**
   ```bash
   cd path/to/CS_project
   ```

3. **Create the virtual environment**
   ```bash
   python3 -m venv cs-venv
   ```

4. **Activate the virtual environment**
   ```bash
   source cs-venv/bin/activate
   ```
   After activation, you should see `(cs-venv)` at the beginning of your command prompt.

5. **Install required packages**
   ```bash
   pip install -r requirements.txt
   ```

6. **Deactivate (when done)**
   ```bash
   deactivate
   ```

### Troubleshooting

- **If `python` command is not found**: Try using `python3` instead
- **If `venv` module is not found**: Install it using `pip install virtualenv` or install Python with pip included
- **Permission errors on Linux/Mac**: You may need to use `sudo` for system-wide installations, but it's better to use a virtual environment without sudo

### Notes

- Always activate the virtual environment before working on the project
- The `cs-venv` folder contains the virtual environment and should not be committed to version control (it's typically in `.gitignore`)
- If you need to recreate the environment, simply delete the `cs-venv` folder and follow the steps again
