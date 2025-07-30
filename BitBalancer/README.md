BitBalancer is a digital logic module that evaluates the balance between the number of '1's and '0's in a binary word. It's designed to be used in digital systems that require data integrity checks, signal calibration, or statistical analysis of binary sequences.

Features:

Accepts an N-bit binary input

Counts the number of logical '1's

Detects whether the input is balanced, one-heavy, or zero-heavy

Fully combinational (or sequential — based on your implementation)

Easy to integrate in testbenches or communication modules

Applications:

Digital Signal Processing (DSP): Ensure data uniformity in encoded signals

Error Detection: Identify imbalanced bit streams

Cryptography & Encoding: Validate pseudo-random sequences or bit entropy

Testing: Used in simulation for verifying data balance properties

How It Works:

Takes an input vector (e.g., 8-bit or 16-bit).

Counts the number of '1's using a population counter.

Compares the count with half the width of the input:

Equal → Balanced

More 1's → One-heavy

More 0's → Zero-heavy

Files:

bitbalancer.sv: Source code of the BitBalancer module

bitbalancer_tb.sv: Testbench with sample inputs

bitbalancer.vcd: Waveform dump for GTKWave analysis

