# GFG_30
---
Difficulty: Medium  
Source: 160 Days of Problem Solving  
Tags:
  - Searching
  - Divide and Conquer
---

# 🚀 _Day 30. Search in Rotated Sorted Array_ 🧠


The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/batch/gfg-160-problems/track/searching-gfg-160/problem/search-in-a-rotated-array4618)


## 💡 **Problem Description:**

Given a sorted (in ascending order) and rotated array `arr` of distinct elements which may be rotated at some point and given an element `key`, the task is to find the index of the given element `key` in the array `arr`. The whole array `arr` is given as the range to search. Rotation shifts elements of the array by a certain number of positions, with elements that fall off one end reappearing at the other end.

**Note:** 0-based indexing is followed & returns -1 if the key is not present.

## 🔍 **Example Walkthrough:**

Input:
```
arr[] = [5, 6, 7, 8, 9, 10, 1, 2, 3], key = 10
```
Output:
```
5
```
Explanation:
10 is found at index 5.

## 🎯 **My Approach:**

1. **Initialization:**
- Use a linear search approach to iterate through the array `arr`.

2. **Search for Key:**
- Iterate through each element in the array from `i = 0` to `n-1` (where `n` is the size of the array).
- Compare each element with the `key`.
- If a match is found, return the index `i`.
- If the end of the array is reached without finding the `key`, return -1.

## 🕒 **Time and Auxiliary Space Complexity** 

- **Expected Time Complexity:** O(n), as we iterate through the array once to find the `key`.
- **Expected Auxiliary Space Complexity:** O(1), as we only use a constant amount of additional space.

## 📝 **Solution Code**
## Code (Python)

```python
class Solution:
    def search(self, arr, key):
        n = len(arr)
        for i in range(n):
            if arr[i] == key:
                return i
        return -1
```
