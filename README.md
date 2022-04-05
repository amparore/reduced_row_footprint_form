# reduced_row_footprint_form
This repository hosts a simple Python code that computed the *reduced row footprint form of* (RRFF) a matrix.
The RREF is similar to the *reduced row echelon form* (RREF), with the difference that
 * Only values below each row leading entry are zeroed in RRFF, while in RREF every element above and below are zeroed.
 * Values above each trailing entry are zeroed.

The code defines a single function `rrff` that takes in input an arbitrary $N \times M$ matrix and return its RRFF. The canonical form is define dover the integers, i.e. leading entries are not necessarily $1$, but instead the greates common divisor of each row is made to be $1$.

The code implements the theory described in the paper:
```
``The footprint form of a matrix: definition, properties, and an application'',
Amparore, Elvio G. and Ciardo, Gianfranco and Miner, Andrew S., Linear Algebra and its Applications, To appear.
```