# Contains Duplicate

- **LeetCode:** [#217 – Contains Duplicate](https://leetcode.com/problems/contains-duplicate/)
- **Difficulty:** Easy
- **Topic:** Arrays & Hashing
- **Pattern:** Set

## Problem Understanding

Given an integer array `nums`, determine whether any value appears at least twice.

Return `True` if duplicates exist, otherwise return `False`.

## Approach

Used Python's built-in `set()` to eliminate duplicate elements.

A set stores only unique values, making it possible to detect duplicates by comparing the lengths of the original list and the resulting set.

## Logic

1. Convert the input list into a set.
2. Compare the length of the original list with the set.
3. If the set contains fewer elements, duplicates were present.
4. Otherwise, all elements are unique.

## Complexity Analysis

- **Time Complexity:** O(n) average — Creating the set requires processing the input elements.
- **Space Complexity:** O(n) — The set may store up to n unique elements.

## Key Learnings

- Understanding Python sets and uniqueness.
- Using `set()` for duplicate detection.
- Understanding the difference between O(1) length retrieval and O(n) set construction.
- Analysing time and auxiliary space complexity.

## Result

- **Status:** Accepted
- **Test Cases:** 71/71 (verify against your actual submission)
