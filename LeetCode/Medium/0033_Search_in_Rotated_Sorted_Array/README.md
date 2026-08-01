# 33. Search in Rotated Sorted Array

Difficulty: Medium
Language: 1class Solution:
2    def search(self, nums: List[int], target: int) -> int:
3        n = len(nums)
4        low,high = 0, n - 1
5        
6
7        while low <= high:
8            mid = (low + high) // 2 
9            if nums[mid] == target:
10                return mid 
11            if nums[mid] <= nums[high]:
12                if nums[mid] <= target <= nums[high]:
13                    low = mid + 1
14                else:
15                    high = mid - 1
16
17            else:
18                if nums[low] <= target <= nums[mid]:
19                    high = mid - 1
20                else:
21                    low = mid + 1 
22        return -1
23
24
Runtime: 0
ms
Memory: 19.42
MB

Problem
https://leetcode.com/problems/search-in-rotated-sorted-array/

Tags
Array
Binary Search

## Approach
The problem "Search in Rotated Sorted Array" is solved using an optimal algorithmic approach in 1class Solution:
2    def search(self, nums: List[int], target: int) -> int:
3        n = len(nums)
4        low,high = 0, n - 1
5        
6
7        while low <= high:
8            mid = (low + high) // 2 
9            if nums[mid] == target:
10                return mid 
11            if nums[mid] <= nums[high]:
12                if nums[mid] <= target <= nums[high]:
13                    low = mid + 1
14                else:
15                    high = mid - 1
16
17            else:
18                if nums[low] <= target <= nums[mid]:
19                    high = mid - 1
20                else:
21                    low = mid + 1 
22        return -1
23
24. The implementation efficiently handles edge cases and processes data with suitable data structures to meet LeetCode runtime (0
ms) constraints.

## Time Complexity
O(N)

## Space Complexity
O(1)
