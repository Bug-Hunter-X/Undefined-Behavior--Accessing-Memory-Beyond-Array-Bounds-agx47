# C Undefined Behavior Example: Array Out-of-Bounds Access

This repository demonstrates a common error in C programming: accessing memory beyond the bounds of an array. This leads to undefined behavior, which can manifest in various ways, including crashes, unexpected results, or seemingly random behavior.

The `bug.c` file contains the erroneous code. The `bugSolution.c` file shows how to correct the issue.

**Understanding the Problem**

In C, arrays are contiguous blocks of memory. When an array is declared, the compiler allocates a specific amount of memory to store its elements. Trying to access memory locations outside this allocated block results in undefined behavior. The behavior can vary depending on the compiler, system, and other factors. 

**How to Fix It**

The solution involves ensuring all array accesses are within the valid index range (0 to array_size - 1).  Bounds checking is crucial for safe and reliable code.