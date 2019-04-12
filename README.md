# hw60 wrap up binary search


## Logarithms

*y=log<sub>2</sub>x* means raising 2 to the *y*th power to get *x*.
Its graph is the graph of y=2<sup>2</sup> reflected over y=x.


## Recursive Solution

**Problem**: finding the desired name within the low and high page limits

**Recursive Abstraction**: When I am asked to find the desired name
within the low and high page limits, the recursive abstraction can find the
desired name within the next smaller-sized page limits.

**Binary Expression**: the low limit is greater than the high limit

**Base Case**: If the low limit is greater than the high limit, return -2.

**Recursive Case**: If not,
- Let pageToCheck equal the arithmetic mean of low and high.
- Let comparison equal the result of comparing the desired name to the
name on pageToCheck.
- If the comparison returns 0, return pageToCheck. (**Base case**)
- Else if the comparison returns a negative number, the recursive abstraction
can find the desired name within the low limit and pageToCheck-1 (as the
high limit). (**Recursive Abstraction**)
- Else the recursive abstraction can find the desired name within pageToCheck+1
(as the low limit) and the high limit. (**Recursive Abstraction**)






