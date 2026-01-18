# Find Unique Element

**Platform:** CodingNinjas
**Question Number:** 1
**Difficulty:** Medium

## Problem Description

You are given an integer array `arr` of size $N = 2M + 1$. Exactly $M$ values appear twice, and one value appears only once. Return the unique value that occurs exactly once. You can assume a unique element always exists under these conditions.

## Examples

### Sample 1

```
Input:
1            // number of test cases
7            // N
2 3 1 6 3 6 2

Output:
1
```

Explanation: In the array `[2, 3, 1, 6, 3, 6, 2]`, the values `2`, `3`, and `6` each appear twice, and `1` appears once, so the answer is `1`.

### Sample 2

```
Input:
2            // number of test cases
5            // N
2 4 7 2 7
9            // N
1 3 1 3 6 6 7 10 7

Output:
4
10
```

Explanation: In the first test, `2` and `7` appear twice and `4` is unique. In the second test, `1`, `3`, `6`, and `7` appear twice while `10` appears once.

## Constraints

- $1 \le t \le 10^2$
- $0 \le N \le 10^3$
- Array size follows $N = 2M + 1$ with a single unique element.
- Time Limit: 1 second
