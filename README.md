# hw60 wrap binary search


## Logarithms

*count=log<sub>2</sub>x* means *count* is the power to which 2 is raised to get the number *n*.
Its graph is the graph of y=2<sup>x</sup> reflected over y=x.


## Recursive Solution

**Problem**: finding the desired name within the low and high page limits

**Recursive Abstraction**: When I am asked to find the desired name
within the low and high page limits, the recursive abstraction can find the
desired name within the next smaller-sized page limits using these instructions.

**Decision to Binary Expression**: the low limit is greater than the high limit

**Solution to Base Case**: If the low limit is greater than the high limit, return -2.

**Solutions to Recursive Cases**: If the low limit is not greater than the high limit,
- Let pageToCheck equal the arithmetic mean of low and high.
- Let comparison equal the result of comparing the desired name to the
name on pageToCheck.
- If the comparison returns 0, return pageToCheck. (**Solution to Base case**)
- Else if the comparison returns a negative number, the recursive abstraction
can find the desired name within the low limit and pageToCheck-1 (as the
high limit) using these instructions. (**Recursive Abstraction**)
- Else the recursive abstraction can find the desired name within pageToCheck+1
(as the low limit) and the high limit using these instructions. (**Recursive
Abstraction**)






