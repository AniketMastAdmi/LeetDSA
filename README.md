# LeetCode Solutions

Total Solved: 1
Easy: 1
Medium: 0
Hard: 0

Languages
1class Solution:
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

Last Updated
2026-07-24 18:13


## Solved Problems

| # | Title | Difficulty | Language | Synced At |
|---|---|---|---|---|
| 35 | [Search Insert Position](https://github.com/AniketMastAdmi/LeetDSA/blob/main/LeetCode/Easy/0035_Search_Insert_Position/solution.txt) | Easy | 1class Solution:
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
17 | 2026-07-24 |
