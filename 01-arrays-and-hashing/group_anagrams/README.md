# Group Anagrams

- **LeetCode:** [#49 – Group Anagrams](https://leetcode.com/problems/group-anagrams/)
- **Difficulty:** Medium
- **Topic:** Arrays & Hashing
- **Pattern:** Hash Map + Sorting

## Problem Understanding

Given an array of strings, group all anagrams together. Strings containing the same characters with identical frequencies belong to the same group.

## Approach

Used a dictionary to group anagrams based on their sorted character sequences.

Sorting each word produces a common key for words containing the same characters, regardless of their original order.

## Logic

1. Initialize an empty dictionary.
2. Iterate through each word in the input list.
3. Sort the characters of the word and join them into a string to generate a key.
4. If the key does not exist, create an empty list for that group.
5. Append the original word to the corresponding group.
6. Return all dictionary values as a list of lists.

## Complexity Analysis

Let:
- `n` = number of words.
- `k` = maximum length of a word.

- **Time Complexity:** O(n × k log k) — Each word is sorted individually.
- **Space Complexity:** O(n × k) — Stores the grouped words and their keys.

## Key Learnings

- Using dictionaries to group related elements.
- Generating common keys using `sorted()` and `join()`.
- Understanding dictionary methods such as `values()`.
- Applying hash maps to solve grouping problems.
- Understanding sorting-based anagram detection.

## Result

- **Status:** Accepted