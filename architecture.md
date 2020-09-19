# Architecture

- [Introduction](#introduction)
- [Directories and files hierarchy](#directories-and-files-hierarchy)



## Introduction

This document describes basic architecture of drivers for each supported
microcontroller.

Architecture describes:

* how directories and files are organized;
* what a public API should look like, and what it should provide for outside
  callers;
* what should be private and what should be public.

What is the most important, architecture should be flexible and evolutionary.



## Directories and files hierarchy

Hierarchy is the same for each microcontroller model.

stm32f407xx
|
|_system
|   |_include
|       |_stm32f407xx.h
|
|_core
|   |_include
|       |_cortex_m4.h
|
|_peripherals
|   |_include
|       |_adc.h
|       |_clock.h
|       |_dac.h
|       |_dma.h
|       |_gpio.h
|       |_i2c.h
|       |_rtc.h
|       |_spi.h
|       |_uart.h
|   |_source
|       |_adc.c
|       |_clock.c
|       |_dac.c
|       |_dma.c
|       |_gpio.c
|       |_i2c.c
|       |_rtc.c
|       |_spi.c
|       |_uart.c
|
|_linker
|   |_stm32f407xx_linker_script.ld
|
|_startup
|   |_stm32f407xx_startup_code.s

