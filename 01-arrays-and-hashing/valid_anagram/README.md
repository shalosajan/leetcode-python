# Valid Anagram

- **LeetCode:** [#242 – Valid Anagram](https://leetcode.com/problems/valid-anagram/)
- **Difficulty:** Easy
- **Topic:** Arrays & Hashing
- **Pattern:** Frequency Counting (Hash Map)

## Problem Understanding

Given two strings `s` and `t`, determine whether `t` is an anagram of `s`.

Both strings must contain exactly the same characters with identical frequencies, regardless of their order.

## Approach

Used a dictionary to count the frequency of each character in the first string.

Instead of creating another dictionary for the second string, reused the existing dictionary by decrementing character frequencies while iterating through the second string.

## Logic

1. Check whether both strings have the same length.
2. Build a frequency dictionary for the first string.
3. Iterate through the second string.
4. Check whether each character exists in the dictionary.
5. Decrement its frequency.
6. Return `False` if a character is missing or its frequency becomes negative.
7. If all characters are processed successfully, return `True`.

## Complexity Analysis

- **Time Complexity:** O(n) — Both strings are traversed once, with average O(1) dictionary operations.
- **Space Complexity:** O(k) — The dictionary stores frequencies for k distinct characters.

## Key Learnings

- Dictionary-based frequency counting.
- Using `dict.get()` for simplified frequency updates.
- Reusing a frequency dictionary instead of creating another.
- Detecting mismatches using negative frequencies.
- Understanding time and auxiliary space complexity.

## Result

- **Status:** Accepted
