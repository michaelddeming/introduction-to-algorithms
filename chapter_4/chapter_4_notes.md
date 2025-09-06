# Chapter 4 - Divide-and-Conquer

- **Divide-and-Conquer** is a powerful strategy for designing asymptotically efficient algorithms w/ 3 steps:
    1. *Divide* the problem into one or more subproblems that are smaller instances of the same problem.
    2. *Conquer* the subproblems by solving them recursively.
    3. *Combine* the subproblem solutions to form a solution to the original problem.

- **Base Case**: The simplest possible instance of the problem that can be solved directly without further recursion. (The “stop condition.”)
- **Recursive Case**: The step where the problem is reduced into smaller subproblems of the same type, moving it closer to the base case.

- **Recurrence**: An equation that describes a function in terms of its
value on other, typically smaller, arguments.

- 4 Methods for Solving Recurrences:
    1. Substitution Method:
    2. Recursion-tree Method: 
    3. Master Method: 
    4. Akra-Bazzi Method: 

## 4.1 Multiplying Square Matrices

- **Dense Matrix**: Most of the n<sup>2</sup> entries are nonzero.  
    - Meaning we need to store nearly all n<sup>2</sup> entries directly in the *n × n* array.  

- **Sparse Matrix**: Most of the n<sup>2</sup> entries are 0, so the nonzero entries can be stored more compactly than in an *n × n* array.  
    - If the majority of the n<sup>2</sup> entries are 0, we only store the nonzero values.  
        - However, we must also store the **locations (indices)** of these nonzero values so that the matrix can be reconstructed when needed.

![alt text](image.png)

![alt text](image-1.png)

## 4.2 Strassen's Algorithm for Matrix Multiplication