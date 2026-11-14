# Two Sum

- LeetCode: #1
- Difficulty: Easy
- Topic: Arrays & Hashing
- Pattern: Hash Map

## Approach
Used a dictionary to store previously
visited numbers and their indices.

For every number, calculated its complement
using target - num.

Checked whether the complement existed
in the dictionary before storing the
current number.

## Complexity
- Time: O(n)
- Space: O(n)

## Key Learnings
- Using enumerate() to access indices and values.
- Dictionary lookups.
- Complement-based problem solving.
- Handling duplicate values.

## Result
- Accepted
- 66/66 test cases passed