# CSC 301 – Group Assignment: Product of Array Except Self

**Course:** CSC 301 – Data Structures
**Group Leader:** Morenikeji David Olowo (VUG/SEN/24/11362)

## Files

| File | Description |
|------|-------------|
| `ProductOfArrayExceptSelf.java` | Java solution with test cases |
| `diagram.png` | Diagram of the algorithm |
| `members.csv` | Group members and matric numbers |

## Problem

Given an array of integers, return a new array where each element is the product of all the other elements, without using division.

**Example:** `[1, 2, 3, 4]` → `[24, 12, 8, 6]`

## Approach

In a single pass, the solution multiplies each position by the running product of everything to its **left**, and the mirrored position by the running product of everything to its **right**. When the loop ends, every position holds the product of all other elements.

- **Time complexity:** O(n)
- **Space complexity:** O(1) extra space (not counting the output array)

## How to Run

```bash
javac ProductOfArrayExceptSelf.java
java ProductOfArrayExceptSelf
```

**Expected output:**
```
[24, 12, 8, 6]
[0, 0, 9, 0, 0]
```

## Group Members

See [`members.csv`](members.csv).
