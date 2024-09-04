# 6502_Cpu

6502 CPU Emulator - README
Overview

This project is a simple yet comprehensive 6502 CPU emulator built in C++. It emulates the classic 6502 microprocessor, which was used in early computers and gaming consoles like the NES. The project includes the core CPU implementation, a bus to connect memory and peripherals, and a demo application that visualizes the CPU's operations.
Features

    6502 CPU Emulation: Implements the core functionality of the 6502 CPU, including all official opcodes.
    Bus System: A simulated bus that connects the CPU to memory and other peripherals.
    Disassembler: Converts machine code back into assembly instructions for easier debugging and understanding.
    Demo Application: A simple graphical interface to visualize the CPU's execution, built using the olcPixelGameEngine.

Project Structure

    Bus.h: Defines the Bus class that connects the CPU to memory and other devices. It includes methods for reading and writing data on the bus.
    olc6502.h: Contains the definition of the olc6502 class, which represents the 6502 CPU. This file includes the CPU's registers, flags, and the implementation of all the addressing modes and opcodes.
    olc_6502.cpp: Implements the functionality of the olc6502 class and the demo application that uses the olcPixelGameEngine to visualize the CPU's operations.

Files

    Bus.h:
        Defines the Bus class.
        Contains a 64KB array representing the system's RAM.
        Provides methods to read from and write to the bus.

    olc6502.h:
        Defines the olc6502 class.
        Includes the CPU's registers, such as the accumulator, program counter, and status register.
        Implements the 6502's addressing modes and opcodes.
        Includes methods for CPU operations like reset(), irq(), and nmi().

    olc_6502.cpp:
        Implements the CPU's behavior and the demo application.
        Uses the olcPixelGameEngine to visualize CPU status, memory content, and disassembled code.
        Demonstrates the CPU's operation by loading and executing a simple program.

Getting Started
Prerequisites

    C++ Compiler: A modern C++ compiler (e.g., g++, clang++).
    olcPixelGameEngine: Required to compile and run the demo application. Make sure the engine is available and properly linked in your environment.

Installation

    Clone the repository:

    bash

git clone <repository-url>
cd 6502_Cpu

Compile the project:

    Ensure that the olcPixelGameEngine is included in your project.
    Compile the project using your preferred C++ compiler:

    bash

    g++ -o 6502_Cpu olc_6502.cpp -lX11 -lGL -lpthread -lpng -lstdc++fs

Run the demo:

bash

    ./6502_Cpu

Using the Emulator

    SPACE: Step through the execution of instructions.
    R: Reset the CPU.
    I: Trigger an interrupt request (IRQ).
    N: Trigger a non-maskable interrupt (NMI).

Customization

    Logging: Uncomment #define LOGMODE in olc6502.h to enable detailed logging of CPU operations.

Contributing

Contributions are welcome! Feel free to fork the repository, make changes, and submit a pull request.
License

This project is licensed under the MIT License. See the LICENSE file for details.
Acknowledgements

    olcPixelGameEngine: For providing a simple and powerful framework for creating the demo visualization.
    6502.org: For documentation and resources on the 6502 microprocessor.


https://github.com/user-attachments/assets/3567a3df-fdb3-4d19-b5a6-6a5847ea4f92


    
