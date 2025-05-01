# Scheduler: ARM Task Scheduling for Cortex-M3

## Overview

**Scheduler** is a lightweight ARM task scheduling project designed for the ARM Cortex-M3 microcontroller. It aims to provide a basic framework for task scheduling in embedded systems, laying the groundwork for the future integration of FreeRTOS or other task scheduling mechanisms.

This project demonstrates the custom boot-up process and memory management. It also includes basic system initialization and prepares the platform for future enhancements like FreeRTOS-based task scheduling. The project has been tested using **QEMU** for ARM simulation.

### Key Features
- **Custom Boot Process**: Implements system initialization and stack pointer setup.
- **Interrupt Vector Table**: Basic setup for Cortex-M3 interrupt vector table.
- **Lightweight**: No RTOS yet, focusing on foundational components like boot-up.
- **Future Integration**: Designed to be extended with FreeRTOS and task scheduling capabilities.
- **Tested in QEMU**: The project has been successfully tested using QEMU for ARM simulation.

## Getting Started

### Prerequisites
Before building and flashing the project, ensure that you have the following:
- **ARM Cortex-M3 microcontroller** (e.g., STM32 series).
- **ARM GCC Toolchain**: e.g., `arm-none-eabi-gcc`.
- **QEMU** (for simulation of ARM Cortex-M3).
- **Demo video** (`demo.mp4`) demonstrating the task scheduling in the future.

### Installing Dependencies

1. **ARM GCC Toolchain**:
   - You need the **ARM GCC toolchain** to build the project. It can be installed using the following:
     - **Ubuntu/Debian**:
       ```bash
       sudo apt-get update
       sudo apt-get install gcc-arm-none-eabi
       ```
     - **macOS** (via Homebrew):
       ```bash
       brew tap ArmMbed/homebrew-formulae
       brew install arm-gcc-bin
       ```
     - **Windows**:
       Download and install the **GNU Arm Embedded Toolchain** from [ARM's official site](https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/gnu-rm).

2. **QEMU** (for ARM Simulation):
   - To simulate the ARM Cortex-M3 on your machine, you can install QEMU:
     - **Ubuntu/Debian**:
       ```bash
       sudo apt-get install qemu-system-arm
       ```
     - **macOS**:
       ```bash
       brew install qemu
       ```

3. **Make**:
   - You also need **Make** to build the project:
     - **Ubuntu/Debian**:
       ```bash
       sudo apt-get install make
       ```
     - **macOS** (via Homebrew):
       ```bash
       brew install make
       ```
     - **Windows**:
       You can install **Make** via [MinGW](http://www.mingw.org/) or use Windows Subsystem for Linux (WSL).

## Installation and Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mohin22/Scheduler.git
   cd Scheduler
2. **Build the project:**
   ```bash
   make
   ```
3. **Simulate the ARM Cortex-M3 using QEMU:**
   ```bash
   make qemu
   ```
4. **Start the GDB debugger in another terminal:**
   ```bash
   make gdb
   ```
[🎥 Watch demo.mp4](demo.mp4)



   

