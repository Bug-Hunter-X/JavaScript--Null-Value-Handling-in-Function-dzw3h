# JavaScript Null Value Handling Bug

This repository demonstrates a common subtle bug in JavaScript related to null value handling in functions.  The `foo` function is intended to add two numbers, but its handling of null values is incomplete.

## Bug Description

The `foo` function correctly returns 0 if one of the input arguments is null.  However, it does not explicitly handle the case where *both* arguments are null, which could lead to unexpected behavior or errors in certain applications.  A robust function should explicitly address this edge case.

## Solution

The bug is resolved by adding a separate condition explicitly checking if *both* `a` and `b` are null.

## How to Run

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in your preferred JavaScript environment.
3. Run each file to see the output.  Note the difference in handling null values.