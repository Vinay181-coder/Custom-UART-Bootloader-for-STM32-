# Custom UART Bootloader for STM32

This project implements a **bare-metal custom bootloader** for the **STM32F446RE** microcontroller using **register-level C programming**.  
The bootloader validates the application firmware stored at a custom flash memory address, performs **vector table relocation (VTOR)** and **main stack pointer (MSP) reconfiguration**, and safely transfers execution control to the application.

For debugging and status monitoring, **UART2-based serial logging** is integrated to display boot states such as startup, application validation, and firmware handover.  
A separate application image is also included, which verifies successful bootloader handoff through **UART messages and LED toggle output**.

This project demonstrates key embedded systems concepts such as **memory mapping, flash partitioning, boot sequence control, register-level peripheral configuration, and firmware execution handover**.
