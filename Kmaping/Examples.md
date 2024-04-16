# Question 1: Determine the expression for the following K-Maps

## a

| AB/C                  | $ \bar{C}$ | $C$ |
|-----------------------|------------|-----|
| $\bar {A}$ $\bar{B} $ | 0          | 1   |
| $\bar {A}$ $B$        | 0          | 1   |
| $A$ $B$               | 0          | 1   |
| $A$ $\bar {B}$        | 0          | 1   |

C doesn't change, so it is 1. A and B are the same, so it is 0. The expression is C.

This is because the output is 1 when C is 1, regardless of the value of A and B.

Answer = C

## b

| AB/CD                 | $\bar{C}$ $\bar{D}$ | $\bar{C}$ $D$ | $CD$ | $\overline{CD}$ |
|-----------------------|---------------------|---------------|------|-----------------|
| $\bar {A}$ $\bar{B} $ | 0                   | 0             | 0    | 0               |
| $\bar {A}$ $B$        | 0                   | 0             | 0    | 0               |
| $A$ $B$               | 1                   | 1             | 1    | 1               |
| $A$ $\bar {B}$        | 0                   | 0             | 0    | 0               |

AB is 1, so the output is 1. The expression is AB.

Answer = AB

## c

| AB\CD                 | $\bar{C}\bar{D}$ | $\bar{C}D$ | $CD$ | $\overline{CD}$ |
|-----------------------|------------------|------------|------|-----------------|
| $\bar {A}$ $\bar{B} $ | 0                | 0          | 0    | 0               |
| $\bar {A}$ $B$        | 0                | 1          | 1    | 0               |
| $A$ $B$               | 0                | 1          | 1    | 0               |
| $A$ $\bar {B}$        | 0                | 0          | 0    | 0               |

Group the 4 ones,

C is the only column that the state doesn't change.

answer = C

## d

| AB\CD                 | $\bar{C}\bar{D}$ | $\bar{C}D$ | $CD$ | $C\bar{D}$ |
|-----------------------|------------------|------------|------|------------|
| $\bar {A}$ $\bar{B} $ | 0                | 0          | 0    | 0          |
| $\bar {A}$ $B$        | 0                | 0          | 0    | 0          |
| $A$ $B$               | 1                | 0          | 0    | 1          |
| $A$ $\bar {B}$        | 1                | 0          | 0    | 1          |

Answer = A

this is because A covers every 1 on the table.

## e

| AB\CD                 | $\bar{C}\bar{D}$ | $\bar{C}D$ | $CD$ | $C\bar{D}$ |
|-----------------------|------------------|------------|------|------------|
| $\bar {A}$ $\bar{B} $ | 1                | 0          | 0    | 1          |
| $\bar {A}$ $B$        | 0                | 0          | 0    | 0          |
| $A$ $B$               | 0                | 0          | 0    | 0          |
| $A$ $\bar {B}$        | 1                | 0          | 0    | 1          |

Answer = $\bar{B} + \bar{D}$

This is because $\bar{B} \cdot \bar{D}$ covers every 1 on the table.

## Question 2: Determine the expression for the following K-Maps

| A | B | C | D | Z |      |
|---|---|---|---|---|------|
| 0 | 0 | 0 | 0 | 1 | **** |
| 0 | 0 | 0 | 1 | 0 |      |
| 0 | 0 | 1 | 0 | 1 |      |
| 0 | 0 | 1 | 1 | 0 |      |
| 0 | 1 | 0 | 0 | 1 |      |
| 0 | 1 | 0 | 1 | 0 |      |
| 0 | 1 | 1 | 0 | 1 |      |
| 0 | 1 | 1 | 1 | 0 |      |
| 1 | 0 | 0 | 0 | 1 |      |
| 1 | 0 | 0 | 1 | 0 |      |
| 1 | 0 | 1 | 0 | 1 |      |
| 1 | 0 | 1 | 1 | 0 |      |
| 1 | 1 | 0 | 0 | 1 |      |
| 1 | 1 | 0 | 1 | 0 |      |
| 1 | 1 | 1 | 0 | 1 |      |
| 1 | 1 | 1 | 1 | 0 |      |

awsner = $\bar{A} \cdot \bar{C} \cdot \bar{D} + \bar{A} \cdot C \cdot \bar{D} + A \cdot \bar{C} \cdot \bar{D} + A \cdot C \cdot \bar{D} + A \cdot C \cdot D$

This is because the output is 1 when D is 0, regardless of the value of A and C.
