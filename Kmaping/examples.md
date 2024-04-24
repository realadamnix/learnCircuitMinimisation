# Question 1: Determine the expression for the following K-Maps

## a

| AB/C                 | $ \bar{C}$ | $C$ |
|----------------------|------------|-----|
| $\bar {A}$ $\bar{B}$ | 0          | 1   |
| $\bar {A}$ $B$       | 0          | 1   |
| $A$ $B$              | 0          | 1   |
| $A$ $\bar {B}$       | 0          | 1   |

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

D doesn't in the columns, so D
B doesn't in the rows, so B

Answer = BD

## d

| AB\CD                 | $\bar{C}\bar{D}$ | $\bar{C}D$ | $CD$ | $C\bar{D}$ |
|-----------------------|------------------|------------|------|------------|
| $\bar {A}$ $\bar{B} $ | 0                | 0          | 0    | 0          |
| $\bar {A}$ $B$        | 0                | 0          | 0    | 0          |
| $A$ $B$               | 1                | 0          | 0    | 1          |
| $A$ $\bar {B}$        | 1                | 0          | 0    | 1          |

Answer = A

$\bar{D}$ does not change in the columns, so $\bar{D}$
A does not change in the rows, so A

Answer = $A \cdot \bar{D}$

## e

| AB\CD                 | $\bar{C}\bar{D}$ | $\bar{C}D$ | $CD$ | $C\bar{D}$ |
|-----------------------|------------------|------------|------|------------|
| $\bar {A}$ $\bar{B} $ | 1                | 0          | 0    | 1          |
| $\bar {A}$ $B$        | 0                | 0          | 0    | 0          |
| $A$ $B$               | 0                | 0          | 0    | 0          |
| $A$ $\bar {B}$        | 1                | 0          | 0    | 1          |

Answer = $\overline{B} \cdot \overline{D}$

This is because $\overline{B} \cdot \overline{D}$ covers every 1 on the table.

## Question 2: Determine the expression for the following K-Maps

| A | B | C | D | Output |
|---|---|---|---|-------:|
| 0 | 0 | 0 | 0 |      1 |
| 0 | 0 | 0 | 1 |      0 |
| 0 | 0 | 1 | 0 |      1 |
| 0 | 0 | 1 | 1 |      0 |
| 0 | 1 | 0 | 0 |      1 |
| 0 | 1 | 0 | 1 |      0 |
| 0 | 1 | 1 | 0 |      1 |
| 0 | 1 | 1 | 1 |      0 |
| 1 | 0 | 0 | 0 |      1 |
| 1 | 0 | 0 | 1 |      0 |
| 1 | 0 | 1 | 0 |      1 |
| 1 | 0 | 1 | 1 |      0 |
| 1 | 1 | 0 | 0 |      1 |
| 1 | 1 | 0 | 1 |      0 |
| 1 | 1 | 1 | 0 |      1 |
| 1 | 1 | 1 | 1 |      0 |

| AB\CD                 | $\bar{C}\bar{D}$ | $\bar{C}D$ | $CD$ | $C\bar{D}$ |
|-----------------------|:----------------:|------------|------|:----------:|
| $\bar {A}$ $\bar{B} $ |        1         |            |      |     1      |
| $\bar {A}$ $B$        |        1         |            |      |     1      |
| $A$ $B$               |        1         |            |      |     1      |
| $A$ $\bar {B}$        |        1         |            |      |     1      |

Answer = $\bar{A} \cdot \bar{C} \cdot \bar{D} + \bar{A} \cdot C \cdot \bar{D} + A \cdot \bar{C} \cdot \bar{D} + A \cdot C \cdot \bar{D} + A \cdot C \cdot D$

This is because the output is 1 when D is 0, regardless of the value of A and C.




## Question 3: Use a Kmap to simplify C’(A’B’D’ + D) + AB’C + D’

The first step is to expand the expression:

$C' \cdot (A' \cdot B' \cdot D' + D) + A \cdot B' \cdot C + D'$

first you have to create a through table with the values of the expression:

| A | B | C | D | $A' \cdot B' \cdot D' + D$ | $A \cdot B' \cdot C$ | $D'$ | $C' \cdot (A'B'D' + D) + AB'C + D'$ |

| 0 | 0 | 0 | 0 | 1                           | 0                     | 1    | 1                                         |
| 0 | 0 | 0 | 1 | 1                           | 0                     | 0    | 1                                         |
| 0 | 0 | 1 | 0 | 1                           | 0                     | 1    | 1                                         |
| 0 | 0 | 1 | 1 | 1                           | 0                     | 0    | 1                                         |
| 0 | 1 | 0 | 0 | 1                           | 0                     | 1    | 1                                         |
| 0 | 1 | 0 | 1 | 1                           | 0                     | 0    | 1                                         |
| 0 | 1 | 1 | 0 | 1                           | 0                     | 1    | 1                                         |
| 0 | 1 | 1 | 1 | 1                           | 0                     | 0    | 1                                         |
| 1 | 0 | 0 | 0 | 1                           | 0                     | 1    | 1                                         |
| 1 | 0 | 0 | 1 | 1                           | 0                     | 0    | 1                                         |
| 1 | 0 | 1 | 0 | 1                           | 0                     | 1    | 1                                         |
| 1 | 0 | 1 | 1 | 1                           | 0                     | 0    | 1                                         |
| 1 | 1 | 0 | 0 | 1                           | 0                     | 1    | 1                                         |
| 1 | 1 | 0 | 1 | 1                           | 0                     | 0    | 1                                         |
| 1 | 1 | 1 | 0 | 1                           | 1                     | 1    | 1                                         |
| 1 | 1 | 1 | 1 | 1                           | 0                     | 0    | 1                                         |

The expression is 1 when the output is 1, so the expression is 1.


then, we can simplify the expression using a Kmap:

| AB/C                 | $\bar{C}\bar{D}$ | $\bar{C} D$ | $CD$ | $C \bar{D}$ | $C\bar{D}$ |
|----------------------|------------------|-------------|------|-------------|------------|
| $\bar {A}$ $\bar{B}$ | 0                | 1           | 0    | 0           | 0          |
| $\bar {A}$ $B$       | 0                | 1           | 0    | 0           | 0          |
| $A$ $B$              | 0                | 1           | 0    | 0           | 0          |
| $A$ $\bar {B}$       | 0                | 1           | 0    | 0           | 0          |


The expression is C.