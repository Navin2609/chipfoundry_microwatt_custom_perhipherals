# Microwatt Sensor Peripheral Integration

## Project Overview
This project extends the open-source Microwatt POWER CPU core by adding a **custom sensor peripheral**.  
The goal is to demonstrate how Microwatt can interact with the physical world through sensors, making it useful for embedded and IoT applications.

## Problem Statement
While Microwatt provides a functional OpenPOWER CPU core, it lacks dedicated hardware interfaces for real-world sensors.  
In IoT and embedded systems, CPUs must communicate with sensors (temperature, distance, humidity, etc.) through efficient and low-latency hardware blocks.

## Proposed Solution
We propose designing a **custom memory-mapped peripheral** that connects a simple digital sensor (e.g., temperature/humidity or ultrasonic sensor) to Microwatt.  
The peripheral will be integrated into Microwatt’s bus system and made accessible at a fixed memory address.  
A demo application will be developed in C or Micropython running on Microwatt to:
- Continuously read sensor values,
- Display them over UART,
- Trigger LEDs or other actuators based on threshold values.


## Expected Outcome
- A working SoC consisting of Microwatt + custom peripheral.  
- Reproducible testbenches and FPGA synthesis results.  
- A software demo showing live sensor data read by Microwatt.  
- Open-source code and documentation to help others extend Microwatt with their own peripherals.

- <img width="1536" height="1024" alt="ChatGPT Image Sep 21, 2025, 01_00_36 AM" src="https://github.com/user-attachments/assets/2e9843f7-9daa-41c0-bb9e-2f355e88aee4" />

