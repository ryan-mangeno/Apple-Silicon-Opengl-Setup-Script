# GLFW & GLAD Project Setup Script

This script automates the setup of a new project using GLFW and GLAD on macOS. It creates a basic structure for an OpenGL project, allowing you to quickly start coding with GLFW and GLAD, and generates necessary source files, a Makefile, and a default project structure.

![Project Demo](images/Demo.png)

## Prerequisites

Before running the script, ensure you have the following tools installed:

1. **Homebrew**: A package manager for macOS.
   - Install it by following the [Homebrew installation guide](https://brew.sh/).
   
2. **GLFW**: A library for creating windows with OpenGL contexts and managing input.
   - The script automatically checks and installs GLFW via Homebrew if it's not already installed.

3. **GLAD**: An OpenGL loader that handles the loading of OpenGL extensions.
   - The script assumes GLAD is downloaded and placed in the `Downloads` folder.

## Features

- **GLFW Installation**: The script checks if GLFW is installed using Homebrew. If it's not installed, it installs it automatically.

- **GLAD Check**: The script checks if GLAD exists in the `Downloads` folder. If not, it prompts you to download and place GLAD in the folder.

- **Project Structure**:
  - Creates a new project directory with the following subdirectories:
    - `src/`: Contains source files.
    - `build/`: Contains build output.
    - `include/`: Contains header files.
    - `lib/`: Contains library files.

- **Source File Creation**:
  - Prompts you to select between C or C++ for your project language.
  - Creates a `main.c` or `main.cpp` file depending on your choice, with default OpenGL setup code.

    ⚠️*C++ Support is not working propperly , there are linking errors with GLAD*⚠️  **Will be fixed soon**

- **Makefile Generation**:
  - Automatically creates a Makefile that compiles the project using `gcc` or `g++` based on your language choice.
  - Includes necessary flags for GLFW and GLAD.
  - Supports building, cleaning, and running the project with the `make` command.

- **GLFW & GLAD Integration**: The script sets up GLFW and GLAD for use in your project, ensuring that the necessary include paths and libraries are correctly configured.

## Usage

1. Clone or download this repository.
2. Ensure that **Homebrew** and **GLFW** are installed.
3. Download **GLAD** from [glad.dav1d.de](https://glad.dav1d.de/) and place it in your `Downloads` folder.
4. Run the script:

   ```bash
   $ chmod +x applesilicon.sh
   $ ./applesilicon.sh
=======
# GLFW & GLAD Project Setup Script

This script automates the setup of a new project using GLFW and GLAD on macOS. It creates a basic structure for an OpenGL project, allowing you to quickly start coding with GLFW and GLAD, and generates necessary source files, a Makefile, and a default project structure.

## Prerequisites

Before running the script, ensure you have the following tools installed:

1. **Homebrew**: A package manager for macOS.
   - Install it by following the [Homebrew installation guide](https://brew.sh/).
   
2. **GLFW**: A library for creating windows with OpenGL contexts and managing input.
   - The script automatically checks and installs GLFW via Homebrew if it's not already installed.

3. **GLAD**: An OpenGL loader that handles the loading of OpenGL extensions.
   - The script assumes GLAD is downloaded and placed in the `Downloads` folder.

## Features

- **GLFW Installation**: The script checks if GLFW is installed using Homebrew. If it's not installed, it installs it automatically.

- **GLAD Check**: The script checks if GLAD exists in the `Downloads` folder. If not, it prompts you to download and place GLAD in the folder.

- **Project Structure**:
  - Creates a new project directory with the following subdirectories:
    - `src/`: Contains source files.
    - `build/`: Contains build output.
    - `include/`: Contains header files.
    - `lib/`: Contains library files.

- **Source File Creation**:
  - Prompts you to select between C or C++ for your project language.
  - Creates a `main.c` or `main.cpp` file depending on your choice, with default OpenGL setup code.

- **Makefile Generation**:
  - Automatically creates a Makefile that compiles the project using `gcc` or `g++` based on your language choice.
  - Includes necessary flags for GLFW and GLAD.
  - Supports building, cleaning, and running the project with the `make` command.

- **GLFW & GLAD Integration**: The script sets up GLFW and GLAD for use in your project, ensuring that the necessary include paths and libraries are correctly configured.

## Usage

1. Clone or download this repository.
2. Ensure that **Homebrew** and **GLFW** are installed.
3. Download **GLAD** from [glad.dav1d.de](https://glad.dav1d.de/) and place it in your `Downloads` folder.
4. Run the script:

   ```bash
   chmod +x applesilicon.sh
   ./applesilicon.sh

