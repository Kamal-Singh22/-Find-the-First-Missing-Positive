# -Find-the-First-Missing-Positive
Given an unsorted integer array nums, return the smallest missing positive integer.
Explanation:
Replace Invalid Numbers:

Replace all negative numbers, zeros, and numbers greater than n with n + 1, since they cannot be the smallest missing positive.
Marking Presence:

For each valid number 𝑥
x, mark its presence by negating the value at index 𝑥−1x−1 (if 𝑥≤𝑛x≤n).
Identify Missing Positive:

The first index with a positive value indicates the smallest missing positive integer.
Return Default:

If all numbers from 1 to n are present, return n + 1.
