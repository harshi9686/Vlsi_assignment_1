Pulse Tracer is a digital logic module designed to detect and trace clean high pulses from a noisy input signal. It filters out glitches and noise, ensuring that only stable, valid pulses are registered and acted upon. This module is especially useful in FPGA/ASIC designs where reliable pulse detection is critical, such as in event counters, trigger systems, or digital communication interfaces.

Features:
Detects single-cycle clean high pulses

Ignores glitches or spurious transitions

Synchronous design for clocked environments

Easily integrable in larger RTL systems

Use Case:
In noisy environments or when signals come from mechanical switches or asynchronous sources, it’s common to encounter short unwanted spikes. Pulse Tracer ensures that only genuine, stable high pulses are detected.

How It Works:
Input Filtering: Uses a small synchronizer or debounce logic to filter short glitches.

Edge Detection: Detects rising edges of the filtered input.

Pulse Generation: Outputs a single-cycle high pulse when a valid rising edge is detected.

Files:
design.sv: SystemVerilog source code of the Pulse Tracer module

testbench.sv: Testbench to verify functionality and simulate edge cases

pulse_detector.vcd: Waveform file for visualizing behavior in tools like GTKWave

