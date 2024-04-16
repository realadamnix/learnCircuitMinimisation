# Shop question

## Problem Statement

Administrator = always has access

Manager = can only enter with engineer

Engineer = can only enter with manager

Design a combination logic circuit that will allow access to the server room by producing a logic 1 when the above conditions are met.

## Step 1: Truth Table

| $A$ | $M$ | $E$ | $X$ (output) | Boolean   |
|-----|-----|-----|--------------|-----------|
| 1   | 1   | 1   | 1            | A + M + E |
| 1   | 1   | 0   | 0            | A + M     |
| 1   | 0   | 1   | 0            | A + E     |
| 1   | 0   | 0   | 0            | A         |
| 0   | 1   | 1   | 0            | M + E     |
| 0   | 1   | 0   | 0            | M         |
| 0   | 0   | 1   | 0            | E         |
| 0   | 0   | 0   | 0            |           |

## Step 2: Boolean expression to represent each outputted logic 1

$A + M + E \cdot A + M \cdot A + E \cdot A \cdot M + E \cdot M \cdot E \cdot E$

## Step 3: Simplify the Boolean expression

$ A + M + E \cdot A \cdot M \cdot E $