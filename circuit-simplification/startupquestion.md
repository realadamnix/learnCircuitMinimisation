# Shop question

## Problem Statement

Administrator = always has access

Manager = can only enter with engineer

Engineer = can only enter with manager

Design a combination logic circuit that will allow access to the server room by producing a logic 1 when the above conditions are met.

## Step 1: Truth Table

| $A$ | $M$ | $E$ | $X$ (output) | Boolean                         |
|-----|-----|-----|:------------:|---------------------------------|
| 1   | 1   | 1   |      1       | $A \cdot M \cdot E$             |
| 1   | 1   | 0   |      1       | $A \cdot M \cdot \bar{E}$       |
| 1   | 0   | 1   |      1       | $A \cdot \bar{M} \cdot E$       |
| 1   | 0   | 0   |      1       | $A \cdot \bar{M} \cdot \bar{E}$ |
| 0   | 1   | 1   |      1       | $\bar{A}\cdot M \cdot E$        |
| 0   | 1   | 0   |      0       |                                 |
| 0   | 0   | 1   |      0       |                                 |
| 0   | 0   | 0   |      0       |                                 |

## Step 2: Boolean expression to represent each outputted logic 1

$(A \cdot M \cdot E) + (A \cdot M \cdot \bar{E}) + (A \cdot \bar{M} \cdot E) + (A \cdot \bar{M} \cdot \bar{E}) + (\bar{A} \cdot M \cdot E)$

## Step 3: Simplify the Boolean expression

$(A \cdot M \cdot E) + (A \cdot M \cdot \bar{E}) + (A \cdot \bar{M} \cdot E) + (A \cdot \bar{M} \cdot \bar{E}) + (\bar{A} \cdot M \cdot E)$  
$((A \cdot M) \cdot (E + \bar{E})) + ((A \cdot \bar{M}) \cdot (E + \bar{E})) + (\bar{A} \cdot M \cdot E)$
$((A \cdot M) \cdot 1) + ((A \cdot \bar{M}) \cdot 1) + (\bar{A} \cdot M \cdot E)$  
$(A \cdot M) + (A \cdot \bar{M}) + (\bar{A} \cdot M \cdot E)$
$A \cdot (M + \bar{M}) + (\bar{A} \cdot M \cdot E)$
$A \cdot 1 + (\bar{A} \cdot M \cdot E)$
$A + (\bar{A} \cdot M \cdot E)$

RULE: $A \cdot A = A$  
RULE: $A + A = A$  
RULE: $A + \bar{A} = 1$  
RULE: $A \cdot \bar{A} = 0$  

$A + M + E \cdot A + M \cdot A + E \cdot A \cdot M + E \cdot M \cdot E \cdot E$

$A + M \cdot A + E \cdot A + E \cdot A \cdot M + E \cdot M \cdot E \cdot E$

$A  \cdot (M + E)$
