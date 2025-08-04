# Raspberry Pi SenseHAT to Micro:bit Maqueen Control System

## Overview
| **Aspect**        | **Details**                                                          |
|-------------------|----------------------------------------------------------------------|
| **Hardware**      | Raspberry Pi 4B + SenseHAT, BBC micro:bit, Maqueen robot chassis     |
| **Languages**     | Python (OOP), Rust, MicroPython                                      |
| **Communication** | PyBluez (Bluetooth)                                                  |
| **Simulation**    | SenseHAT emulator, micro:bit simulator, robotic simulation platforms |
| **Environment**   | Windows 11 + WSL2 (Ubuntu 24.04), ROS 2 integration planned          |
| **License**       | [GPL-3.0 License](https://www.gnu.org/licenses/gpl-3.0.en.html)      |

## Motivation

### Technical Learning
- Experience with simulators, emulators, embedded systems, and Bluetooth protocols

### Programming Practice
- Apply **object-oriented programming**
- Build **modular** and **extensible** components

### Hybrid Development
- Support for:
  - Python & Rust
  - ROS 2 framework
  - WSL2-based Linux environments

## System Architecture
![System Architecture](<Screenshot 2025-07-02 133425.png>)

## Development Environment
| **Category**       | **Details**                                                    |
|--------------------|----------------------------------------------------------------|
| **OS**             | Windows 11 with WSL2                                           |
| **Languages**      | Python, Rust, MicroPython                                      |
| **Frameworks**     | ROS 2                                                          |
| **Embedded Tools** | PlatformIO (VS Code), PyCharm + MicroPython Plugin, Thonny IDE |
| **Simulators**     | micro:bit simulator                                            |
| **Emulators**      | SenseHAT                                                       |

## Installation & Setup

### Core Software
| Tool/Framework | Installation Guide                                                                 |
|----------------|-------------------------------------------------------------------------------------|
| ROS 2 (Humble) | [ROS 2 Humble Installation](https://docs.ros.org/en/humble/Installation.html)      |
| Python         | [Python for Windows](https://www.python.org/downloads/windows/)                    |
| Rust           | [Rust Setup](https://learn.microsoft.com/en-us/windows/dev-environment/rust/setup) |
| MicroPython    | [MicroPython](https://micropython.org/)                                            |

### IDEs & Tools
| Tool                 | Setup Guide                                                                                             |
|----------------------|---------------------------------------------------------------------------------------------------------|
| Visual Studio Code   | [VS Code Setup](https://code.visualstudio.com/docs/setup/windows)                                       |
| PlatformIO Extension | [PlatformIO for VS Code](https://marketplace.visualstudio.com/items?itemName=platformio.platformio-ide) |
| PyCharm              | [PyCharm Download](https://www.jetbrains.com/pycharm/download/)                                         |
| MicroPython Plugin   | [MicroPython Plugin](https://plugins.jetbrains.com/plugin/26227-micropython-tools)                      |
| Thonny IDE           | [Thonny IDE](https://thonny.org/)                                                                       |

### System Dependencies
| Component | Guide                                                                                                                                                        |
|----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| micro:bit | [Micro:bit Foundation](https://microbit.org/)                                                                                                                |
| WSL2      | [Ubuntu on WSL2](https://documentation.ubuntu.com/wsl/stable/howto/install-ubuntu-wsl2/), [WSL Setup](https://learn.microsoft.com/en-us/windows/wsl/install) |

## Future Vision
- Maintain ROS 2 and Python on Raspberry Pi
- Migrate micro:bit firmware from MicroPython to Rust
- Expand simulation and testing capabilities

## System Description

### Functionality
- Capture joystick input from SenseHAT
- Convert input to directional commands
- Transmit via Bluetooth to micro:bit
- Control Maqueen robot in real-time

### Simulation Support
- SenseHAT emulator for input
- micro:bit simulator for firmware testing
- Robotic platforms for virtual prototyping

### Scalability
- ROS 2-ready architecture
- Compatible with both physical and virtual environments

## Features
- Joystick input capture
- Motion command generation
- Bluetooth communication
- Multi-language support (Python, Rust, MicroPython)
- Hybrid environment compatibility
- Modular architecture
- ROS 2 integratability

## Clone the Repository
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

## micro:bit & Maqueen Robot

### micro:bit Configuration

#### 1. Hardware Setup
- Mount the micro:bit onto the Maqueen chassis.
- Confirm correct battery placement and motor wiring.

#### 2. Firmware Installation
- Flash MicroPython or Rust firmware to the micro:bit.
- Use `.uf2` files for MicroPython or `cargo` for Rust builds.

#### 3. Bluetooth Configuration
- Pair the micro:bit with the Raspberry Pi using PyBluez.
- Define a command protocol to interpret joystick input.

#### 4. Simulation & Emulation
- Use the micro:bit simulator to test firmware logic.
- Use the SenseHAT emulator to simulate joystick input.

#### 5. Language Integration
- Current development focuses on MicroPython and Python for core functionality.
- Rust migration is planned for a future phase.
- Cross-language interoperability will be addressed after system validation.

### Usage Instructions *(Coming Soon)*
Guides for running the system, launching simulators, and controlling the robot will be added as development progresses.

## Testing *(Planned)*
- Unit and integration tests will validate software components.
- Emulator-based testing will simulate input and robot behavior.
- Hardware and simulation testing strategies are under design and will be finalized in later stages.

## Contribution
This project is under active development and not currently accepting external contributions.

Contribution guidelines and issue templates will be published with the initial stable release.
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

## micro:bit & Maqueen Robot

### micro:bit Configuration

#### 1. Hardware Setup
- Mount the micro:bit onto the Maqueen chassis.
- Confirm correct battery placement and motor wiring.

#### 2. Firmware Installation
- Flash MicroPython or Rust firmware to the micro:bit.
- Use `.uf2` files for MicroPython or `cargo` for Rust builds.

#### 3. Bluetooth Configuration
- Pair the micro:bit with the Raspberry Pi using PyBluez.
- Define a command protocol to interpret joystick input.

#### 4. Simulation & Emulation
- Use the micro:bit simulator to test firmware logic.
- Use the SenseHAT emulator to simulate joystick input.

#### 5. Language Integration
- Current development focuses on MicroPython and Python for core functionality.
- Rust migration is planned for a future phase.
- Cross-language interoperability will be addressed after system validation.

### Usage Instructions *(Coming Soon)*
Guides for running the system, launching simulators, and controlling the robot will be added as development progresses.

## Testing *(Planned)*
- Unit and integration tests will validate software components.
- Emulator-based testing will simulate input and robot behavior.
- Hardware and simulation testing strategies are under design and will be finalized in later stages.

## Contribution
This project is under active development and not currently accepting external contributions.

Contribution guidelines and issue templates will be published with the initial stable release.