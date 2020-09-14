# uavcan-template-c

This template project is intended to be used as a started project for developing an [UAVCAN](https://uavcan.org/) node in C using [libcanard](https://github.com/UAVCAN/libcanard) and socketcan as the [Platform-specific component](https://github.com/UAVCAN/platform_specific_components).

The cuurnet code is based on the demo found at the forum post  [Automatic configuration of port identifiers](https://forum.uavcan.org/t/automatic-configuration-of-port-identifiers/840/3) by Pavel Kirienko. The current code only has the heartbeat implemented. If you wish to follow Pavel's demo then uncommenting the relevant code in main.c should be all you to do to start completing the demo.

### Requirements

#### Operating System

This template has been tested to be used on a Debian based Linux distribuition such as Ubuntu and Raspberry Pi OS.

#### IDE's

Visual Studio Code is the intended target IDE. The project depends on CMake for building thus in theory other IDE's could be used.
* Visual Studio Code with:
  * C/C++ Extension
  * CMake Tools Extension
