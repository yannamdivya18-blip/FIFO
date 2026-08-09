# FIFO Memory Design Using Verilog HDL

## Overview

This project implements a synchronous FIFO (First-In First-Out) memory using Verilog HDL. FIFO is a widely used data buffering structure where the first data entered is the first data removed.

## Features

* Parameterized FIFO design
* Separate Read and Write operations
* Full and Empty status flags
* Synchronous operation using a clock
* Verilog testbench for verification

## Files

* `fifo.v` – FIFO design module
* `fifo_tb.v` – Testbench for simulation
* `simulation_results.png` – Waveform screenshot

## FIFO Operation

### Write

Data is stored into FIFO when:

* `wr_en = 1`
* FIFO is not full

### Read

Data is read from FIFO when:

* `rd_en = 1`
* FIFO is not empty

## Status Flags

* **full** = 1 → FIFO cannot accept more data
* **empty** = 1 → FIFO contains no data

## Tools Used

* Verilog HDL
* ModelSim
* Icarus Verilog
* GTKWave

## Simulation Procedure

1. Compile `fifo.v` and `fifo_tb.v`
2. Run simulation
3. Open waveform viewer
4. Verify write and read operations
5. Observe Full and Empty flags

## Applications

* UART Buffers
* Network Routers
* Digital Signal Processing
* Embedded Systems
* FPGA and ASIC Designs

## Results

The FIFO successfully stores incoming data and retrieves it in the same order in which it was written, validating First-In First-Out operation.

## Author

Akula Rajini Yadav

B.Tech – Electronics and Communication Engineering (ECE)
