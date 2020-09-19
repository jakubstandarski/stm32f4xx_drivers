# STM32F4xx: Drivers

- [Overview](#overview)
    - [Goal](#goal)
    - [What inside](#what-inside)
    - [Supported microcontrollers](#supported-microcontrollers)
- [Software requirements](#system-requirements)



## Overview

### Goal

Goal of this project is to create completely new drivers for STM32F4xx
microcontrollers from scratch based only on available documents, datasheets,
reference manuals and schematics.


### What inside

This project doesn't use any third-party packages like STM32CubeF4 provided by
ST, or CMSIS provided by ARM. Each part of the driver is made completely from
scratch.

Anyway, this shouldn't be a problem, because this project provides everything 
you need for building any kind of embedded system application. You can find
there system files (similar to the ones from CMSIS package), startup
codes, linker scripts, makefiles and the most important peripherals drivers
(e.g. GPIO, SPI, I2C, UART, ADC, Timer, etc.).


### Supported microcontrollers

Supported microcontrollers (so far):

* STM32F407xx
* STM32F413xx



## Software requirements

* **OS**: Ubuntu 20.04
* **Toolchain**: GNU Arm Embedded Toolchain 9-2020-q2-update 9.3.1
* **Additional software**: OpenOCD

