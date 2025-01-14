# Unexpected Behavior with Mutable Variables in F#

This repository demonstrates a common error in F# related to the behavior of mutable variables when passed to functions.  In F#, mutable variables are passed by reference, which can lead to unintended side effects if not handled correctly. The `bug.fs` file showcases this issue, while `bugSolution.fs` provides a corrected approach.

## Problem

The `swap` function attempts to swap the values of two mutable variables, `x` and `y`. However, because of the pass-by-reference behavior, the function directly modifies the original variables, resulting in an output that might be unexpected.

## Solution

The solution involves creating a new tuple containing the swapped values and returning it. This avoids directly modifying the original variables.

## Running the Code

1. Make sure you have the F# compiler installed.
2. Compile the code using the F# compiler (fsc.exe).
3. Run the compiled executable.