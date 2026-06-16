# CAN Protocol Analyzer

Designed and implemented a CAN Protocol Analyzer in C to simulate and monitor Controller Area Network (CAN) communication. Developed core modules including Frame Generation, Message Filtering, Arbitration Logic, Error Detection, and Bus Monitoring. Verified functionality through software simulation and analysis of CAN frame transmission and reception.


## Overview

Designed and implemented a software-based CAN Protocol Analyzer inspired by automotive communication systems. The project focuses on understanding CAN bus architecture, frame structure, arbitration mechanisms, message filtering, and error handling. The analyzer simulates the transmission and reception of CAN messages and provides insight into communication behavior commonly used in automotive and industrial embedded systems.


## Project Objectives

* Understand the fundamentals of CAN communication.
* Simulate CAN frame transmission and reception.
* Analyze message arbitration mechanisms.
* Implement frame filtering and error detection.
* Gain practical experience with automotive communication protocols.


## Key Features

### Developed a CAN protocol analyzer supporting:

* CAN frame generation
* Standard and Extended CAN IDs
* Message transmission and reception
* Bus arbitration mechanism
* Message filtering
* Error detection and handling
* Frame decoding and analysis
* Bus load monitoring
* Logging and timestamp generation

### Designed and integrated core modules including:

* CAN Frame Generator
* Transmit Module
* Receive Module
* Arbitration Logic
* Message Filter
* Error Detection Module
* Bus Monitor
* Logging Module

### Implemented frame types:

* Data Frame
* Remote Frame
* Error Frame
* Overload Frame

### Supported CAN features:

* Standard CAN (11-bit Identifier)
* Extended CAN (29-bit Identifier)
* Message Priority Arbitration
* CRC Verification
* Acknowledgment Handling

### Functional capabilities:

* Frame encoding and decoding
* Message filtering by ID
* Arbitration simulation
* Error frame detection
* Logging of transmitted and received frames
* Bus utilization analysis


## System Architecture

The CAN Protocol Analyzer consists of frame generation, arbitration logic, message filtering, error detection, and monitoring modules. Messages are processed and analyzed to simulate communication behavior on a CAN bus.


## CAN Protocol Analyzer Architecture

<img width="2368" height="4200" alt="image" src="https://github.com/user-attachments/assets/ba10536c-c180-4949-bb5c-9d2e51d3d35e" />



## Core Modules

### CAN Frame Generator

Constructs CAN frames including identifier, control field, data field, CRC, acknowledgment, and end-of-frame segments.

### Transmit Module

Handles message transmission onto the simulated CAN bus.

### Receive Module

Receives and decodes incoming CAN frames.

### Arbitration Logic

Implements non-destructive bitwise arbitration to determine bus access priority.

### Message Filter

Accepts or rejects frames based on configured identifiers.

### Error Detection Module

Detects communication errors using CRC checks and frame validation mechanisms.

### Bus Monitor

Tracks CAN traffic and provides statistics for analysis.

### Logging Module

Records transmitted and received messages with timestamps.


## Supported Frame Types

The analyzer supports the following CAN frame types:

* Data Frame
* Remote Frame
* Error Frame
* Overload Frame


## Arbitration Mechanism

The CAN protocol uses non-destructive bitwise arbitration. Nodes with lower identifier values obtain higher priority and continue transmission while lower-priority nodes wait for the next bus availability.


## Directory Structure

```text
CAN-Protocol-Analyzer
│
├── src
│   ├── can_frame.c
│   ├── can_frame.h
│   ├── transmitter.c
│   ├── transmitter.h
│   ├── receiver.c
│   ├── receiver.h
│   ├── arbitration.c
│   ├── arbitration.h
│   ├── filter.c
│   ├── filter.h
│   ├── error_handler.c
│   ├── error_handler.h
│   ├── logger.c
│   ├── logger.h
│   └── main.c
│
├── include
│
├── test
│   ├── frame_test.c
│   ├── arbitration_test.c
│   └── filter_test.c
│
├── docs
│   ├── architecture.png
│   ├── frame_structure.png
│   ├── arbitration_flow.png
│   └── message_trace.png
│
└── README.md
```


## Verification

Performed functional verification using software-based test cases to validate:

* Frame generation and decoding
* Standard and Extended CAN IDs
* Arbitration behavior
* Message filtering operation
* Error frame generation
* CRC validation
* Transmission and reception mechanisms


## Tools & Technologies

* C Programming
* CAN Protocol
* Embedded Systems
* GCC
* VS Code
* Git
* GitHub
* Automotive Communication Concepts


## Applications

This project architecture can be applied in:

* Automotive Electronic Control Units (ECUs)
* Battery Management Systems (BMS)
* EV Charging Systems
* Industrial Automation
* Motor Control Systems
* IoT and Sensor Networks


## Learning Outcomes

Through this project, I gained practical understanding of:

* CAN frame structure
* Arbitration mechanisms
* Message priority handling
* Standard and Extended CAN identifiers
* Error detection and fault handling
* Message filtering techniques
* Bus monitoring and traffic analysis
* Automotive communication concepts


## Outcome

Successfully demonstrated the operation of a CAN Protocol Analyzer and gained hands-on experience in CAN communication, frame handling, arbitration mechanisms, message filtering, and error detection. This project strengthened practical knowledge of automotive communication protocols and embedded networking concepts.


## Future Enhancements

The following features can be incorporated to further enhance the analyzer:

* CAN FD support
* J1939 protocol support
* DBC file parsing
* Graphical user interface
* Real-time bus visualization
* Data logging to CSV
* Message statistics and diagnostics
* Error injection capability
* SocketCAN integration
* STM32 hardware-based implementation

