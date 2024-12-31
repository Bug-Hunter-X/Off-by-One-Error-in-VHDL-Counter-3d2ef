# VHDL Counter Bug
This repository demonstrates a common off-by-one error in a simple VHDL counter and its solution. The buggy counter might not reset correctly under specific circumstances, leading to inaccurate counting and potentially causing issues in larger designs.

## Bug Description
The `buggy_counter.vhd` file contains a VHDL implementation of a counter that increments on the rising edge of the clock and resets when a reset signal is high. However, there's a potential off-by-one error in the reset condition, leading to improper reset behavior under particular clock conditions. This can manifest as the counter not resetting to zero when expected.

## Solution
The `fixed_counter.vhd` file shows how to fix the counter. The solution ensures the correct reset behavior and eliminates the off-by-one error. The changes are carefully explained in comments within the code.

## How to Reproduce
1. Clone this repository.
2. Simulate both `buggy_counter.vhd` and `fixed_counter.vhd` using your preferred VHDL simulator (e.g., ModelSim, GHDL). 
3. Apply various clock and reset signals to observe the different behaviors.

The simulation should clearly demonstrate the counter's incorrect behavior in `buggy_counter.vhd` and the corrected behavior in `fixed_counter.vhd`.