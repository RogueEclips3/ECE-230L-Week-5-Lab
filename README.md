# Lab 05 - Combinatorial Logic

By Joshua Richmond and Dylan Duljkovic

## Lab Summary

In this lab, we learned how to create more complex Verilog code. Specifically, we learned
how to separate modules into different files and how to connect different inputs and outputs
to different modules. For example, we had a module called "circuit_a" in one file, and routed
its output to another module in a different file called "circuit_b".

## Lab Questions

### 1 - Explain the role of the Top Level file.

The top level file in Verilog is basically the equivalent of the entry point for a standard programming
language. The top level file is what connects all other modules together into one circuit.

### 2 - Explain the function of the Constraints file.

The constraints file maps the inputs and outputs of the top level file to actual pins on the board
that we operate on. For example, on the Basys3 board, the V17 is switch 0, and the constraints file
that we use maps that to the input "sw[0]".

### 3 - Was the selection of Minterm and Maxterm correct for each circuit? What would you have chosen?

Personally, we thought that it would have been better to choose Minterm for both Circuit A and Circuit B.
Although both the minterm and maxterm provided the exact same equation for Circuit A, we thought the
minterm would have been better because the minterm only had a single group, rather than the maxterm
with two groups. As for Circuit B, we thought the minterm was the correct choice simply because there would
have been way too many groups with the maxterm.