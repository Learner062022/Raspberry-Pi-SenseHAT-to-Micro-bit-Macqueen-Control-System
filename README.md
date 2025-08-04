# Raspberry-Pi-SenseHAT-to-Micro-bit-Macqueen-Control-System

## Description

This project builds a modular robotics control system using:

### Hardware Components
- **Raspberry Pi** with SenseHAT joystick
- **BBC micro:bit**
- **Maqueen robot chassis**

### Software Technologies
- **Python** (object-oriented design)
- **Bluetooth communication** via PyBluez
- **MicroPython or Rust** for micro:bit firmware

### Functionality
- Captures joystick input from SenseHAT
- Converts input into directional motion commands
- Sends commands wirelessly to micro:bit via Bluetooth
- Controls Maqueen robot in real-time

### Simulation Support
- SenseHAT emulator for joystick input
- micro:bit simulator for firmware testing
- Robot simulation platforms for virtual testing

### Scalability
- Designed for future integration with **ROS 2**
- Supports both **physical** and **virtual** environments

## Motivation
This project was driven by the following goals:

### Technical Learning
- Gain hands-on experience with:
  - Simulators and emulators
  - Embedded systems and robotics hardware
  - Bluetooth communication protocols

### Programming Practice
- Apply **object-oriented programming** principles in a robotics context
- Develop **modular** and **extensible** software components

### Hybrid Development
- Build a system compatible with:
  - **Python and Rust**
  - **ROS 2 framework**
  - **WSL2-based Linux environments** on Windows

### Future Vision
While ROS 2 within a WSL2 environment and Python on the Raspberry Pi 4B remain constant, the long-term goal is to migrate the micro:bit from MicroPython to Rust. 

## Development Environment
- **OS:** Windows 11 with WSL2
- **Languages:** Python, Rust, MicroPython
- **Frameworks:** ROS 2
- **Tools:** SenseHAT emulator, micro:bit simulators

## Hardware Requirements
- Raspberry Pi 4B
- SenseHAT
- BBC micro:bit
- Maqueen robot

## Software Stack
- Python 3.x
- PyBluez
- SenseHAT library
- ROS 2

## Features 
- Joystick input
- Motion commands
- Bluetooth communication
- Multi-language support
- Hybrid environment compatability
- Modular architecture
- ROS 2 integratability

## Installation & Setup

### Pre-requisites

#### ROS 2
- [ROS 2 Humble Installation Guide](https://docs.ros.org/en/humble/Installation.html)

#### micro:bit
- [Micro:bit Educational Foundation](https://microbit.org/)

#### MicroPython
- [MicroPython](https://micropython.org/)

#### Python
- [Python Installation Guide (Windows)](https://www.python.org/downloads/windows/)

#### Visual Studio Code
- [Visual Studio Code Setup](https://code.visualstudio.com/docs/setup/windows)

#### Rust
- [Rust Setup on Windows](https://learn.microsoft.com/en-us/windows/dev-environment/rust/setup)

#### WSL2
- [Install Ubuntu on WSL2](https://documentation.ubuntu.com/wsl/stable/howto/install-ubuntu-wsl2/)
- [WSL Installation Guide](https://learn.microsoft.com/en-us/windows/wsl/install)

### Clone the Repo
```bash
git clone https://github.com/Learner062022/Amaze.git
cd Amaze
```

### Install Dependencies

#### Python
```bash
pip install sense-hat pybleuz
```

#### Rust
```bash
cargo build
```

#### ROS 2
```bash
sudo apt update
rosdep update
rosdep install --from-paths src --ignore-src -r -y
```

#### MicroPython

## micro:bit & Maqueen Robot

### micro:bit Configuration

#### 1. Hardware Setup
- Connect micro:bit to Maqueen chassis.
- Ensure batttery and motor wiring is correct.

#### 2. Firmware Installation
- Flash MicroPython or Rust firmware to micro:bit.
- Use `utf` files or `cargo` for Rust builds.

#### 3. Bluetooth Configuration
- Pair micro:bit with Raspberry Pia via PyBluez.
- Define command protocol for joystick input.

#### 4. Simulation & Emulation
- Use micro:bit simulator for testing logic.
- SenseHAT emulator for joystick input.

#### 5. Integration with Python & Rust
- Integration details will be shared during the Rust migration phase.
- Current development prioritizes core functionality and system verification using MicroPython and Python.
- Cross-language interoperability will be addressed after core objectives are met.

### How to Use
Instructions for running the system, launching simulators and controlling the robot will be added as development progresses.

## Testing
Unit and integration tests, as well as emulator-based validation, will be implemented. The testing strategies for hardware and simulation environments are yet to be determined.

## System Architecture
![alt text](<Screenshot 2025-07-02 133425.png>)

## Contribution
This project is currently under active development and is not accepting external contributions at this time.

Contribution guidelines and issue templates will be made available once the initial version is complete.

## License
This project is licensed under [GPL-3.0 License](https://www.gnu.org/licenses/gpl-3.0.en.html).