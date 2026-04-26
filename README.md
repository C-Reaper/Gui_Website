# Project README

## Overview
The project is a C/C++ application that demonstrates the creation of a simple GUI for displaying various interactive components such as labels, buttons, progress bars, scrollbars, sliders, text fields, and rotatable elements. The GUI is defined using an XML-like syntax in `Main.alxml`.

## Features
- **Labels**: Display static text.
- **Buttons**: Interactable elements that can trigger actions.
- **Progress Bars**: Indicators of progress with customizable speed.
- **Scrollbars**: For scrolling through content or to select items.
- **Sliders**: Controls for adjusting values within a range.
- **Text Fields**: Input fields for entering text.
- **Rotatable Elements**: UI components that can rotate.

## Project Structure
### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools
- Libraries needed in specific projects (example given WINAPI, X11, ALSA)

## Build & Run
### Linux
1. **Build**:
    ```sh
    cd <Project>
    make -f Makefile.linux all
    ```
2. **Execute**:
    ```sh
    make -f Makefile.linux exe
    ```

### Windows
1. **Build**:
    ```sh
    cd <Project>
    make -f Makefile.windows all
    ```
2. **Execute**:
    ```sh
    make -f Makefile.windows exe
    ```

### Wine (Linux Cross Compile for Windows)
1. **Build**:
    ```sh
    cd <Project>
    make -f Makefile.wine all
    ```
2. **Execute**:
    ```sh
    make -f Makefile.wine exe
    ```

### WebAssembly (Emscripten or wasmtime)
1. **Build**:
    ```sh
    cd <Project>
    make -f Makefile.web all
    ```
2. **Run**:
    ```sh
    make -f Makefile.web exe
    ```

The build process compiles the `Main.c` file and any other associated header files to produce an executable for the target platform. The project includes multiple Makefiles for different platforms, ensuring compatibility across Linux, Windows, Wine (for cross-compilation), and WebAssembly environments.