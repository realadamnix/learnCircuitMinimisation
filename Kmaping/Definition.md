# What is K-Mapping in Karnaugh Map?

## Definition

K-mapping is a technique used to simplify boolean expressions. It is also known as Kavanagh Map. It is a graphical representation of a truth table. It is used to simplify boolean expressions by grouping the min-terms or max-terms that have the same output value.

The K-Map is a two-dimensional grid with rows and columns representing the input variables. The cells in the grid represent the output of the boolean expression for each combination of input variables. The K-Map is used to identify patterns in the output values and simplify the boolean expression. The K-Map is a useful tool for simplifying complex boolean expressions and reducing the number of gates in a circuit.

## Example

For example, consider the boolean expression $\bar{A}B + A\bar{B} + AB$. The K-Map for this expression is as follows:

| A | B | Q | name  |
| - | - | - | ----- |
| 0 | 0 | 0 | *w* |
| 0 | 1 | 1 | *x* |
| 1 | 0 | 1 | *y* |
| 1 | 1 | 1 | *z* |

|             | $\bar{B}$ | $B$ |
| ----------- | ----------- | ----- |
| $\bar{A}$ | *w*       | *x* |
| $A$       | *y*       | *z* |

|             | $\bar{B}$ | $B$ |
| ----------- | ----------- | ----- |
| $\bar{A}$ |             | 1     |
| $A$       | 1           | 1     |

$A + B$

${\bar{A} \cdot \bar{B}}  = {\bar{A}} + {\bar{B}} = A + B$

The simplified expression is A XOR B.

## Example 3

Here is a truth table for a specific three-input logic circuit:

| A | B | C | Output |
| - | - | - | :----: |
| 0 | 0 | 0 |   1   |
| 0 | 0 | 1 |   1   |
| 0 | 1 | 0 |   0   |
| 0 | 1 | 1 |   1   |
| 1 | 0 | 0 |   0   |
| 1 | 0 | 1 |   1   |
| 1 | 1 | 0 |   0   |
| 1 | 1 | 1 |   0   |

Complete the following Karnaugh  map, according to the values found in the above truth table:

| AB\C | 0 | 1 |
| ---- | - | - |
| 00   | 1 | 1 |
| 01   |   | 1 |
| 11   |   |   |
| 10   |   | 1 |

The K-Map is as follows:
$\overline{AB}+ \bar{B}C + \bar{A}C$

## Explanation

The K-Map is a graphical representation of a truth table. It is used to simplify boolean expressions. The K-Map is a two-dimensional grid with rows and columns representing the input variables. The cells in the grid represent the output of the boolean expression for each combination of input variables. The K-Map is used to identify patterns in the output values and simplify the boolean expression. The K-Map is a useful tool for simplifying complex boolean expressions and reducing the number of gates in a circuit.

## [youtube](https://www.youtube.com/watch?v=RO5alU6PpSU) Examples

### Example 1

| A | B | C | F |
|---|---|---|:-:|
| 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 0 |
| 0 | 1 | 0 | 1 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 0 | 1 |
| 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 0 |

KMap:

| C\AB | 00 | 01 | 11 | 10 |
| ---- | -- | -- | -- | -- |
| 0    | 0  | 1  | 1  | 1  |
| 1    | 0  | 0  | 0  | 1  |

$B\bar{C}+ A\bar{B} = A\bar{B} + B\bar{C}$

$F = A\bar{B} + B\bar{C}$

### Example 2

| A | B | C | F |
|---|---|---|:-:|
| 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 |
| 0 | 1 | 0 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 1 |
| 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 0 |

| BC\A | 0 | 1 |
| ---- | - | - |
| 00   |   | 1 |
| 01   | 1 | 1 |
| 11   | 1 |   |
| 10   |   | 1 |

$F= A\bar{B} + \bar{A}C + A\bar{C} $

### Example 3

| CD\AB | 00 | 01 | 11 | 10 |
| ----- | -- | -- | -- | -- |
| 00    | 0  | 0  | 1  | 0  |
| 01    | 0  | 0  | 1  | 1  |
| 11    | 0  | 0  | 0  | 1  |
| 10    | 1  | 1  | 0  | 0  |

$F = \bar{A}C\bar{D} + AB\bar{C} + A\bar{B}D$

## Example 4

| CD\AB | 00 | 01 | 11 | 10 |
| ----- | -- | -- | -- | -- |
| 00    | 1  | 0  | 0  | 0  |
| 01    | 1  | 0  | 1  | 1  |
| 11    | 1  | 0  | 1  | 1  |
| 10    | 1  | 0  | 0  | 0  |

$F = \overline{AB} + AD$
