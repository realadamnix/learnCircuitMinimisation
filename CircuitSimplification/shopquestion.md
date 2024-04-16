# Shop question 

## Problem Statement

manager (M) = can only enter if the owner is present

owner (O) = can always enter

salesperson (S) = can enter if the manager is present

customer (C) = can enter if the owner is present


Design a combination logic circuit that will allow access by producing a logic 1 when the above conditions are met.

## Step 1: truth table

| M | O | S | C | X (output)    | Boolean |
|---|---|---|---|---------------|---------|
| 1 | 1 | 1 | 1 | M + O + S + C | 1       |
| 1 | 1 | 1 | 0 | M + O + S     | 1       |
| 1 | 1 | 0 | 1 | M + O + C     | 1       |
| 1 | 1 | 0 | 0 | M + O         | 1       |
| 1 | 0 | 1 | 1 |               |         |
| 1 | 0 | 1 | 0 |               |         |
| 1 | 0 | 0 | 1 |               |         |
| 1 | 0 | 0 | 0 |               |         |
| 0 | 1 | 1 | 1 | O + S + C     | 1       |
| 0 | 1 | 1 | 0 | O + S         | 1       |
| 0 | 1 | 0 | 1 | O + C         | 1       |
| 0 | 1 | 0 | 0 | O             | 1       |
| 0 | 0 | 1 | 1 |               |         |
| 0 | 0 | 1 | 0 |               |         |
| 0 | 0 | 0 | 1 |               |         |
| 0 | 0 | 0 | 0 |               |         |


## Step 2: Boolean expression to represent each outputted logic 1

O .O + O \cdot S + O \cdot C + O \cdot S \cdot C + M + M \cdot O + M \cdot S + M \cdot C + M \cdot S \cdot C