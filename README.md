# LeetCode 304 - Range Sum Query 2D - Immutable

## Problem Statement

Given a 2D matrix, handle multiple queries to calculate the sum of all elements inside a rectangular region.

The rectangle is defined by its top-left corner `(row1, col1)` and bottom-right corner `(row2, col2)`.

## Example

### Input

```text
matrix = [
  [3, 0, 1, 4, 2],
  [5, 6, 3, 2, 1],
  [1, 2, 0, 1, 5],
  [4, 1, 0, 1, 7],
  [1, 0, 3, 0, 5]
]

sumRegion(2, 1, 4, 3)
```

### Output

```text
8
```

## Approach

Use a **2D Prefix Sum Matrix**.

Each prefix value stores the sum of all elements from the top-left corner to that position. This allows rectangular sums to be calculated in constant time.

## Algorithm

1. Create a prefix sum matrix.
2. Calculate cumulative sums for every cell.
3. For each query, use the four relevant prefix values.
4. Add and subtract them using the 2D prefix sum formula.
5. Return the calculated sum.

## Time Complexity

* Initialization: `O(m × n)`
* Each `sumRegion` query: `O(1)`

## Space Complexity

`O(m × n)`

## Key Concepts

* 2D Prefix Sum
* Matrix
* Range Sum
* Preprocessing

## Language

Python

## LeetCode Details

* **Problem:** 304
* **Title:** Range Sum Query 2D - Immutable
* **Difficulty:** Medium

## Author

**T. Nandhini Reddy**

GitHub: `242t605119-dotcom`
