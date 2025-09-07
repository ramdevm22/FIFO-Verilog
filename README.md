# FIFO-Verilog
### First-In-First-Out Verilog Design
### Project Description :
This repository contains a synchronous First-In, First-Out (FIFO) queue implemented in Verilog. It's a fundamental digital circuit for buffering data, useful in systems where data needs to be temporarily stored and retrieved in the same order it was written.

This particular design uses a single clock for all operations, ensuring simple and stable data handling. It's built with a memory array and manages data flow using a single address pointer to indicate the current memory location.

### Key Features :
Synchronous Design: All read and write operations are synchronized to a single clock edge.

Fixed-Depth Memory: The FIFO uses a memory array of 16 elements, each capable of storing an 8-bit value.

Status Flags:

full: A signal that asserts when the FIFO reaches its maximum capacity of 16 elements.

empty: A signal that asserts when the FIFO contains no data.

Simple Implementation: The FIFO uses a single addr register to control both read and write operations, moving data through the array in a sequential, "shuffling" manner during a read.
