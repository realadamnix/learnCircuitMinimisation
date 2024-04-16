# Cash room problem

## Problem statement

Suppose the cash room at a store has access restricted to certain
employees, each of whom has a key, which produces a logic 1 at inputs to
an unlocking circuit.

Only the store manager (M) can enter alone. The assistant manager (A) and
the cashier (C) also have access, but only when accompanied by each other,
or by the store manager. Design a combination logic circuit that will allow
access by producing a logic 1 when the above conditions are met.

## Step 1: truth table

| $A$ | $M$ | $C$ | $X$ (output) | Boolean   |
|-----|-----|-----|--------------|-----------|
| 0   | 0   | 0   | 0            |           |
| 0   | 0   | 1   | 0            |           |
| 0   | 1   | 0   | 1            | M         |
| 0   | 1   | 1   | 0            | M + C     |
| 1   | 0   | 0   | 1            |           |
| 1   | 0   | 1   | 0            | A + C     |
| 1   | 1   | 0   | 0            | A + M     |
| 1   | 1   | 1   | 1            | A + C + M |

## Step 2: Boolean expression to represent each outputted logic 1

$X = M + M \cdot C + A\cdot C + A \cdot M + A \cdot C \cdot M$

## Step 3: Simplify the Boolean expression

$X = M + M \cdot C + A\cdot C + A \cdot M + A \cdot C \cdot M$

$X = M + A \cdot C + A \cdot M + A \cdot C \cdot M$

$X = M + A \cdot M + A \cdot C + A \cdot C \cdot M$

$X = M + A \cdot C + A \cdot C \cdot M$

$X = M + A \cdot C \cdot M + A \cdot C$

$X = M + A \cdot C$
