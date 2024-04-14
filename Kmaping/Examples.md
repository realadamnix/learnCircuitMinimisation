
# Question 1: Determine the expression for the following K-Maps

## a

|      | C' | C |
|------|----|---|
| A'B' | 0  | 1 |
| A'B  | 0  | 1 |
| A B  | 0  | 1 |
| A B' | 0  | 1 |

C doesn't change, so it is 1. A and B are the same, so it is 0. The expression is C.

This is because the output is 1 when C is 1, regardless of the value of A and B.

Answer = C

## b

|      | C' | C | CD | CD' |
|------|----|---|----|-----|
| A'B' | 0  | 0 | 0  | 0   |
| A'B  | 0  | 0 | 0  | 0   |
| A B  | 1  | 1 | 1  | 1   |
| A B' | 0  | 0 | 0  | 0   |

AB is 1, so the output is 1. The expression is AB.

Answer = AB

## c

| AB\CD | $\bar{C}\bar{D}$ | $\bar{C}D$ | $CD$ | $C\bar{D}$ |
|-------|------|-----|----|-----|
| A'B'  | 0    | 0   | 0  | 0   |
| A'B   | 0    | 1   | 1  | 0   |
| A B   | 0    | 1   | 1  | 0   |
| A B'  | 0    | 0   | 0  | 0   |

Group the 4 ones,

- The columns $\bar{C}D$ and $CD$.  $D$ is common to both columns, so $D$
- The rows $\bar{A}B$ and $AB$.  $B$ is common to both rows, so $B$

$F = B \cdot D$

This is because C is part of C and CD in the k-map.

Answer = C
