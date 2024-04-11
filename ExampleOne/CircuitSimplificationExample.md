# Circuit simplificationExample

## Step1:Write a Boolean expression for the circuit

The circuit is shown below.

![JPG](CircuitsSimplification.jpg)
We have three inputs A, B, and C.

We will deal with the diagram in 3 steps.  Step 1, the first 3 gates taking inputs from A, B, C
The result of the first 3 gates are

- `And1` = AB
- `Or1`= B+C
- `And2`BC

Step 2, calculate the next gate `And3`, which takes inputs from `Or1` and `And2`.

`And3` = `Or1` * `And2`
`And3` = (B+C) * BC

Step 3, calculate the final gate `Or2`, which takes inputs from `And1` and `And3`.

`Or2` = `And1` + `And3`
`Or2` = AB + (B+C) * BC

The final expression is AB + (B+C) * BC

| A | B | C | `And1`<br/>AB | `And2`<br/>BC | `Or1`<br/>B+C | `And3`= `Or1`*`And2`<br/>(B+C) * BC | `Q`<br/>AB + (B+C) * BC |
|---|---|---|----|----|-----|------------|-----------------|
| 0 | 0 | 0 | 0  | 0  | 0   | 0          | 0               |
| 0 | 0 | 1 | 0  | 0  | 1   | 0          | 0               |
| 0 | 1 | 0 | 0  | 0  | 1   | 0          | 0               |
| 0 | 1 | 1 | 0  | 1  | 1   | 1          | 1               |
| 1 | 0 | 0 | 0  | 0  | 0   | 0          | 0               |
| 1 | 0 | 1 | 0  | 0  | 1   | 0          | 0               |
| 1 | 1 | 0 | 1  | 0  | 1   | 0          | 1               |
| 1 | 1 | 1 | 1  | 1  | 1   | 1          | 1               |

```plaintext

(B+C) * BC

Next Gate is

(B+C) * BC + AB


## Step2:Use Boolean simplification to reduce this expression

= AB + BC (B + C)

= AB + BBC + BCC

= AB + BC + BC

= AB + BC

= BC(A + C)

![JPG](ThroughTableForCircuitsSimplification.jpg)
```
