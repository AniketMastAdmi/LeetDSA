# 35. Search Insert Position

Difficulty: Easy
Language: 1class Solution:
2    def searchInsert(self, nums: List[int], target: int) -> int:
3        n = len(nums)
4        low, high = 0, n-1 
5        lb = n 
6
7        while low <= high:
8            mid = (low + high) // 2
9            # lb = mid 
10            if nums[mid] >= target:
11                lb = mid
12                high = mid - 1
13            else:
14                low = mid + 1
15
16        return lb
17
Runtime: 0 ms
Memory: N/A

Problem
https://leetcode.com/problems/search-insert-position/

Tags
Array
Binary Search

## Approach
The problem "Search Insert Position" is solved using an optimal algorithmic approach in 1class Solution:
2    def searchInsert(self, nums: List[int], target: int) -> int:
3        n = len(nums)
4        low, high = 0, n-1 
5        lb = n 
6
7        while low <= high:
8            mid = (low + high) // 2
9            # lb = mid 
10            if nums[mid] >= target:
11                lb = mid
12                high = mid - 1
13            else:
14                low = mid + 1
15
16        return lb
17. The implementation efficiently handles edge cases and processes data with suitable data structures to meet LeetCode runtime (0 ms) constraints.

## Time Complexity
O(N)

## Space Complexity
O(1)
