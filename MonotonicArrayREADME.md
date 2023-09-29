# leet-day76

# Is Monotonic

## Problem Description

An array is monotonic if it is either monotone increasing or monotone decreasing.

An array `nums` is monotone increasing if for all `i <= j`, `nums[i] <= nums[j]`. An array `nums` is monotone decreasing if for all `i <= j`, `nums[i] >= nums[j]`.

You are given an integer array `nums`. Your task is to determine whether the given array is monotonic or not. Return `true` if the array is monotonic, otherwise return `false`.

## Examples

### Example 1:

**Input:**

```cpp
nums = [1, 2, 2, 3]
```

**Output:**

```cpp
true
```

**Explanation:**

The given array is monotone increasing because for all `i <= j`, `nums[i] <= nums[j]`.

### Example 2:

**Input:**

```cpp
nums = [6, 5, 4, 4]
```

**Output:**

```cpp
true
```

**Explanation:**

The given array is monotone decreasing because for all `i <= j`, `nums[i] >= nums[j]`.

### Example 3:

**Input:**

```cpp
nums = [1, 3, 2]
```

**Output:**

```cpp
false
```

**Explanation:**

The given array is neither monotone increasing nor monotone decreasing.

## Constraints

- `1 <= nums.length <= 105`
- `-105 <= nums[i] <= 105`

## Solution

This problem can be solved efficiently by iterating through the array once and checking whether it's monotone increasing or monotone decreasing. We maintain two counts, `increasing` and `decreasing`, and increment them as we find increasing or decreasing sequences in the array. If either count remains zero throughout the loop, the array is monotonic.

## Complexity Analysis

- Time complexity: O(n), where n is the length of the input array `nums`.
- Space complexity: O(1), as we only use a constant amount of additional space.

