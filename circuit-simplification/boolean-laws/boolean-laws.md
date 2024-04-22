
# Boolean Law

- The laws of Boolean algebra are similar in some ways to those of standard algebra, but in some cases Boolean laws are unique. 
- This is because when logic is applied to digital circuits, any variable such as A can only have two values 1 or 0, whereas in standard algebra A can have many values.

## Commutative Laws

In a group of variables connected by operators AND or OR, the order of the variables does not matter.

1a. Boolean addition (OR): A+B = B+A

1b. Boolean multiplication (AND): A•B = B•A

**Associative Laws ![ref1]**

The order of calculation can be changed without affecting the result (Change which terms are in brackets or remove brackets). 

**Note**: This is **only OK** so long as all signs (+ or •) are the same.

2a. Boolean addition (OR): (A+B)+C = A+(B+C) = A+B+C

2b. Boolean Multiplication (AND): (A•B)•C = A•(B•C) = A•B•C = ABC

**Distributive Laws ![ref1]**

The same answer is arrived at when multiplying (ANDing) a variable by a group of bracketed variables added (ORed) together, as when each multiplication (AND) is performed separately.

Law 3a is similar to factoring in normal algebra, but law 3b is unique to Boolean algebra because unlike normal algebra, where A x A=A2, in Boolean algebra A•A = A.

3a.  A•(B+C) = A•B+A•C

3b.  A+(B•C) = (A+B) • (A+C) 3c.  A + AB = A + B![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.002.png)

**Identity Laws ![ref1]**

In Rule 4a, when the variable A is ANDed with logic 1 (called the Identity Element for the AND operator), the variable ANDed with 1 retains its identity.

4a. A•1 = A![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.003.png)

Rule 4b, shows that the Identity Element for the OR operator is 0, and any variable ORed with 0 it retains its identity.![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.004.png)

4b. A+0 = A

**Identity Laws ![ref1]**

5a and 5b show how by ‘forcing the Identity Element’, (in B column of the truth tables) to the opposite states to those used in 4a and 4b, produces an output that is the same as the Identity Element.

5a. A•0 = 0 ![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.005.png)5b. A+1 = 1 

**Identity Laws ![ref1]**

6a and 6b show that ANDing or ORing two identical variables, produces an output equal to a single variable, showing that one of the variables is redundant, a useful rule when simplifying Boolean equations.

6a. A•A = A ![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.006.png)6b. A+A = A 

**Complement Law ![ref1]**

Any variable ORed with its inverse is 1

7a. A + Ā = 1

Any variable ANDed with its inverse is 0

7b. A • Ā = 0

![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.007.png)

**Reduction ![ref1]**

When a single variable (A) is ANDed with itself OR a second variable (A+B), the result is equal to the single variable.

8a. A•(A+B) = A![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.008.png)

When a single variable (A) is ORed with itself AND a second variable (A•B), the result is equal to the single variable.

8b. A+(A•B) = A![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.009.png)

**Reduction ![ref1]**

When a single variable (A) is ORed with itself OR a second variable (A+B), the single variable disappears.

8c. A+(A+B) = (A+B)![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.010.png)

When a single variable (A) is ANDed with itself AND a second variable (A•B), the single variable disappears.

8d. A•(A•B) = (A•B) ![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.011.png)

**Duality Rules ![ref1]**

It is possible to derive additional identities by obtaining the Dual of an identity.

This involves changing the AND operators to OR and the OR operators to AND. Additionally any 0s are changed to 1s and 1s to 0s.

![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.012.png)

**Duality Rules ![ref1]**

The duality rule can be used to change a logic expression containing both AND and OR elements to its equivalent dual expression. ![](Aspose.Words.fdffbd40-6329-4e64-ad32-c121cedb19ce.013.png)

For example, the  table shows that  A•(B+C) is the  same as A+(B•C). 

**Simplifying Boolean Equations ![ref1]**

- A matter of choosing the most appropriate law or rule to reduce the expression step by step.
- If the resulting minimisation is correct, the minimised equation and the original equation should give identical output columns when truth tables for the original and minimised circuits are compared.

**Simplifying Boolean Equations ![ref1]**

- Boolean algebraic methods are normally used on logic circuits with just a few gates and only two or three inputs, as it becomes more difficult and cumbersome when more gates or inputs are involved.
- Which laws are applied to change an equation, and in what order, is a matter of practice and intuition.

**Simplifying Boolean Equations ![ref1]**

- This method involves looking at the original complex equation and selecting a law that will simplify a particular part, so obtaining a simpler equation, and then choosing another law that will simplify the equation further, and so on until the equation can no longer be made simpler.
- There is no simple algorithm to specify the order of steps to be taken and several routes may be taken to reach the goal of a simplified and ideally minimised circuit.

