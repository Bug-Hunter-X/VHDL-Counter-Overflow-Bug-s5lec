# VHDL Counter Overflow Bug

This repository demonstrates a common error in VHDL code: an integer counter that doesn't explicitly handle overflow conditions.  The `counter_bug.vhdl` file contains the erroneous code.  The correct version is in `counter_solution.vhdl`.

The bug arises because the counter's behavior is undefined when it reaches its maximum value (15 in this case).  A robust solution would explicitly check for the maximum value and handle the overflow explicitly, either by wrapping around or saturating.

This example highlights the importance of carefully considering the potential range of variables in VHDL and explicitly handling boundary conditions to prevent unexpected behavior and ensure predictable operation.