# uavcan-template-c

This template project is intended to be used as a started project for developing an [UAVCAN](https://uavcan.org/) node in C using [libcanard](https://github.com/UAVCAN/libcanard) and socketcan as the [Platform-specific component](https://github.com/UAVCAN/platform_specific_components).

### Requirements

#### Operating System

This template has been tested to be used on a Debian based Linux distribuition such as Ubuntu and Raspberry Pi OS.

#### IDE's

Visual Studio Code is the intended target IDE. The project depends on CMake for building thus in theory other IDE's could be used.
* Visual Studio Code with:
  * C/C++ Extension
  * CMake Tools Extension